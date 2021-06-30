<template>
   <div class="pizza_row_item montanara">
      <figure class="pizza_row_item_photo">
          <img :src=" require('../assets/images/' + product_data.image) " class="image">
      </figure>
    <div class="pizza_row_item_sub">
      <h1>{{product_data.name}}</h1>
      <p>от {{product_data.price}} руб.</p>
      <button @click="addToCart">В корзину</button>
      <p></p>
  </div>
</div>
</template>

<script>
export default {
  name: "cartItem",
  props: {
      product_data: {
          type: Object,
          default() {
              return {}
          }
      }
  },
  data() {
      return {}
  },
  methods: {
    addToCart() {
      this.$emit('addToCart', this.product_data)
    }
  },
};
</script>

<style>
.pizza_row_item {
  width: 25%;
  margin-left: 30px;
  margin-right: 30px;
}
@media screen and (max-width: 800px) {
    .pizza_row_item {
         width: 34%;
         margin-left: 30px;
         margin-right: 30px;
}
.pizza_row_item_sub p {
     font-size: calc(9px + 16 * (100vw / 1920)) !important;
}
.pizza_row_item_sub button {
    margin-top: 7px;
    padding: 3px 13px 3px 13px !important;
}
}
@media screen and (max-width: 439px) {
    .pizza_row_item {
         width: 60%;
         margin-left: 30px;
         margin-right: 30px;
}
}
.pizza_row_item_sub {
  background-color: black;
  color: white;
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  height: 130px;
  border-radius: 0 0 60px 40px;
  width: 100%;
  position: relative;
  bottom: 37px;
}
.pizza_row_item_sub h1 {
  font-size: calc(9px + 16 * (100vw / 1920));
  text-align: center;
}
.pizza_row_item_sub p {
  color: #5c5c5c;
  font-size: calc(7px + 16 * (100vw / 1920));
  text-align: center;
  margin-top: 3px;
}
.pizza_row_item_sub button {
    margin-top: 7px;
    padding: 3px 18px 3px 18px;
}
</style>