<template>
  <div class="cart">
      <div class="cart_link_to_app"><a href="#carth">Корзина: {{CART.length}}</a></div>
          <h1 id="carth">Корзина</h1>
       <cartAddItem 
         v-for="(item, index) in cart_data"
         :key="item.article"
         :cart_item_data="item"
         @deleteFromCart="deleteFromCart(index)"
         @increment="increment(index)"
         @decrement="decrement(index)"
       />
       <div class="cart_total">
           <p class="cart_total_name">Всего:</p>
           <p>{{cartTotalCost}} руб.</p>
       </div>
  </div>
</template>

<script>
import cartAddItem from './cart-add-item.vue'
import {mapActions, mapGetters} from 'vuex'

export default {
    name: "cart",
    components: {
        cartAddItem
    },
    props: {
        cart_data: {
            type: Array,
            default() {
                return []
            }
        }
    },
    data() {
        return {}
    },
 computed: {
    ...mapGetters([
        'PRODUCTS',
        'CART'
    ]),
    cartTotalCost() {
        let result = []

        if (this.cart_data.length) {
           for (let item of this.cart_data) {
            result.push(item.price * item.quantity);
        }
          result = result.reduce(function(sum, el) {
            return sum + el;
        })  
           return result;
      } else {
          return 0;
      }
    }
},
    methods: {
        ...mapActions([
            'DELETE_FROM_CART',
            'INCREMENT_CART_ITEM',
            'DECREMENT_CART_ITEM'
        ]),
        deleteFromCart(index) {
            this.DELETE_FROM_CART(index);
        },
        increment(index) {
            this.INCREMENT_CART_ITEM(index);
        },
        decrement(index) {
            this.DECREMENT_CART_ITEM(index);
        }
    }
}
</script>

<style scoped>
    .cart h1 {
        text-align: center;
        margin: 30px 0 30px 0;
    }
    .cart_link_to_app {
        position: fixed;
        top: 10px;
        right: 10%;
        padding: 16px;
        border: solid 1px #aeaeae;
        background-color: black;
        opacity: 0.9;
        text-decoration: none;
        color: orange;
    }
    .cart_link_to_app a {
        text-decoration: none;
    }
    .cart_link_to_app a:visited {
        color: orange;
    }
    .cart_total {
        position: fixed;
        bottom: 0;
        right: 0;
        left: 0;
        padding: 18px;
        display: flex;
        justify-content: center;
        color: black;
        background-color: orange;
        font-size: 21px;
    }
    .cart_total_name {
        margin-right: 12px;
    }
</style>
