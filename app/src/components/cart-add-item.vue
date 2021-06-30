<template>
  <div class="cart-add-item">
      <img :src=" require('../assets/images/' + cart_item_data.image) " class="image">
          <div class="cart-add-item_info">
              <p>{{cart_item_data.name}}</p>
              <p>{{cart_item_data.price}} руб.</p>
              <p>{{cart_item_data.article}}</p>
          </div>   
          <div class="cart_item_quantity">
             <p>Кол-во:</p>
               <span>
                 <span class="quantity_btn" @click="decrementItem">-</span>
                    {{cart_item_data.quantity}}
                 <span class="quantity_btn" @click="incrementItem">+</span>
               </span>
          </div>
              <button class="remove_btn" @click="deleteFromCart">Удалить</button>       
      </div>
</template>

<script>

export default {
    name: "cartAddItem",
    data() {
        return {}
    },
    methods: {
        deleteFromCart() {
            this.$emit('deleteFromCart');
        },
        decrementItem() {
            this.$emit('decrement');
        },
        incrementItem() {
            this.$emit('increment');
        }
    },
    props: {
        cart_item_data: {
            type: Object,
            default() {
                return {}
            }
        }
    },
    components: {},
}
</script>

<style scoped>
    .cart-add-item h1 {
        margin-top: 25px;
        text-align: center;
    }
    .cart-add-item {
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        flex-wrap: nowrap;
        margin: 12px auto 12px auto;
        width: 60%;
        border: 1px solid black;
        padding: 10px;
        border-radius: 10px;
        box-shadow: 3px 3px 1px gray;
    }
    .cart-add-item img {
        width: 15%;
        height: 80px;
    }
    .quantity_btn {
        cursor: pointer;
        padding: 0 7px 0 7px;
        border: 1px solid gray;
        margin: 0 4px 0 4px;
        border-radius: 4px;
    }
    .remove_btn {
        padding: 2px 4px 2px 4px;
        border-radius: 3px;
        border: 1px solid black;
    }
</style>