<template>
  <div id="app">
    <div class="content">
      <section>
        <div class="header">
           <nav class="header_nav">
              <div class="header_nav_logo">
                        <figure class="header_nav_logo_container">
                            <img src="../src/assets/images/logo_final.png" class="image_logo" alt="FirePizza" />
                        </figure>
                    </div>

                   <!-- Меню-бургер -->
                    <div class="burger-menu">
                        <div class="burger-menu-icon">
                            <svg height="36px" viewBox="0 -66 335.628 335" width="36px"
                                xmlns="http://www.w3.org/2000/svg">
                                <path
                                    d="m328.628906 188.3125h-321.628906c-3.867188 0-7 3.136719-7 7 0 3.867188 3.132812 7 7 7h321.628906c3.863282 0 7-3.132812 7-7 0-3.863281-3.136718-7-7-7zm0 0" />
                                <path
                                    d="m328.628906 94.3125h-321.628906c-3.867188 0-7 3.136719-7 7 0 3.867188 3.132812 7 7 7h321.628906c3.863282 0 7-3.132812 7-7 0-3.863281-3.136718-7-7-7zm0 0" />
                                <path
                                    d="m328.628906.3125h-321.628906c-3.867188 0-7 3.136719-7 7 0 3.867188 3.132812 7 7 7h321.628906c3.863282 0 7-3.132812 7-7 0-3.863281-3.136718-7-7-7zm0 0" />
                            </svg>
                        </div>
                    </div>

                <div class="header_nav_links">
                        <div class="header_nav_links_container">
                            <a class="header_nav_link active" href="#">Меню</a>
                            <a class="header_nav_link" href="../delivery/delivery.html">Доставка</a>
                            <svg class="header_nav_link" id="regular" enable-background="new 0 0 24 24" height="36px"
                                viewBox="0 0 24 24" width="36px" xmlns="http://www.w3.org/2000/svg">
                                <path
                                    d="m12.145 19.5c3.472 0 2.234-2.198 2.502-2.83-.004-.472-.008-.926.008-1.202.22.062.739.325 1.811 1.367 1.655 1.67 2.078 2.665 3.415 2.665h2.461c.78 0 1.186-.323 1.389-.594.196-.262.388-.722.178-1.438-.549-1.724-3.751-4.701-3.95-5.015.03-.058.078-.135.103-.175h-.002c.632-.835 3.044-4.449 3.399-5.895.001-.002.002-.005.002-.008.192-.66.016-1.088-.166-1.33-.274-.362-.71-.545-1.299-.545h-2.461c-.824 0-1.449.415-1.765 1.172-.529 1.345-2.015 4.111-3.129 5.09-.034-1.387-.011-2.446.007-3.233.036-1.535.152-3.029-1.441-3.029h-3.868c-.998 0-1.953 1.09-.919 2.384.904 1.134.325 1.766.52 4.912-.76-.815-2.112-3.016-3.068-5.829-.268-.761-.674-1.466-1.817-1.466h-2.461c-.998 0-1.594.544-1.594 1.455 0 2.046 4.529 13.544 12.145 13.544zm-8.09-13.499c.217 0 .239 0 .4.457.979 2.883 3.175 7.149 4.779 7.149 1.205 0 1.205-1.235 1.205-1.7l-.001-3.702c-.066-1.225-.512-1.835-.805-2.205l3.508.004c.002.017-.02 4.095.01 5.083 0 1.403 1.114 2.207 2.853.447 1.835-2.071 3.104-5.167 3.155-5.293.075-.18.14-.241.376-.241h2.461.01c-.001.003-.001.006-.002.009-.225 1.05-2.446 4.396-3.189 5.435-.012.016-.023.033-.034.05-.327.534-.593 1.124.045 1.954h.001c.058.07.209.234.429.462.684.706 3.03 3.12 3.238 4.08-.138.022-.288.006-2.613.011-.495 0-.882-.74-2.359-2.23-1.328-1.292-2.19-1.82-2.975-1.82-1.524 0-1.413 1.237-1.399 2.733.005 1.622-.005 1.109.006 1.211-.089.035-.344.105-1.009.105-6.345 0-10.477-10.071-10.636-11.996.055-.005.812-.002 2.546-.003z" />
                            </svg>
                            <svg class="header_nav_link" height="36px" viewBox="0 0 511 511.9" width="36px"
                                xmlns="http://www.w3.org/2000/svg">
                                <path
                                    d="m510.949219 150.5c-1.199219-27.199219-5.597657-45.898438-11.898438-62.101562-6.5-17.199219-16.5-32.597657-29.601562-45.398438-12.800781-13-28.300781-23.101562-45.300781-29.5-16.296876-6.300781-34.898438-10.699219-62.097657-11.898438-27.402343-1.300781-36.101562-1.601562-105.601562-1.601562s-78.199219.300781-105.5 1.5c-27.199219 1.199219-45.898438 5.601562-62.097657 11.898438-17.203124 6.5-32.601562 16.5-45.402343 29.601562-13 12.800781-23.097657 28.300781-29.5 45.300781-6.300781 16.300781-10.699219 34.898438-11.898438 62.097657-1.300781 27.402343-1.601562 36.101562-1.601562 105.601562s.300781 78.199219 1.5 105.5c1.199219 27.199219 5.601562 45.898438 11.902343 62.101562 6.5 17.199219 16.597657 32.597657 29.597657 45.398438 12.800781 13 28.300781 23.101562 45.300781 29.5 16.300781 6.300781 34.898438 10.699219 62.101562 11.898438 27.296876 1.203124 36 1.5 105.5 1.5s78.199219-.296876 105.5-1.5c27.199219-1.199219 45.898438-5.597657 62.097657-11.898438 34.402343-13.300781 61.601562-40.5 74.902343-74.898438 6.296876-16.300781 10.699219-34.902343 11.898438-62.101562 1.199219-27.300781 1.5-36 1.5-105.5s-.101562-78.199219-1.300781-105.5zm-46.097657 209c-1.101562 25-5.300781 38.5-8.800781 47.5-8.601562 22.300781-26.300781 40-48.601562 48.601562-9 3.5-22.597657 7.699219-47.5 8.796876-27 1.203124-35.097657 1.5-103.398438 1.5s-76.5-.296876-103.402343-1.5c-25-1.097657-38.5-5.296876-47.5-8.796876-11.097657-4.101562-21.199219-10.601562-29.398438-19.101562-8.5-8.300781-15-18.300781-19.101562-29.398438-3.5-9-7.699219-22.601562-8.796876-47.5-1.203124-27-1.5-35.101562-1.5-103.402343s.296876-76.5 1.5-103.398438c1.097657-25 5.296876-38.5 8.796876-47.5 4.101562-11.101562 10.601562-21.199219 19.203124-29.402343 8.296876-8.5 18.296876-15 29.398438-19.097657 9-3.5 22.601562-7.699219 47.5-8.800781 27-1.199219 35.101562-1.5 103.398438-1.5 68.402343 0 76.5.300781 103.402343 1.5 25 1.101562 38.5 5.300781 47.5 8.800781 11.097657 4.097657 21.199219 10.597657 29.398438 19.097657 8.5 8.300781 15 18.300781 19.101562 29.402343 3.5 9 7.699219 22.597657 8.800781 47.5 1.199219 27 1.5 35.097657 1.5 103.398438s-.300781 76.300781-1.5 103.300781zm0 0" />
                                <path
                                    d="m256.449219 124.5c-72.597657 0-131.5 58.898438-131.5 131.5s58.902343 131.5 131.5 131.5c72.601562 0 131.5-58.898438 131.5-131.5s-58.898438-131.5-131.5-131.5zm0 216.800781c-47.097657 0-85.300781-38.199219-85.300781-85.300781s38.203124-85.300781 85.300781-85.300781c47.101562 0 85.300781 38.199219 85.300781 85.300781s-38.199219 85.300781-85.300781 85.300781zm0 0" />
                                <path
                                    d="m423.851562 119.300781c0 16.953125-13.746093 30.699219-30.703124 30.699219-16.953126 0-30.699219-13.746094-30.699219-30.699219 0-16.957031 13.746093-30.699219 30.699219-30.699219 16.957031 0 30.703124 13.742188 30.703124 30.699219zm0 0" />
                            </svg>
                        </div>
                    </div>
                    
         <!--           <div class="header_delivery">
                        <div class="header_delivery_container">
                            <div class="header_delivery_icon">
                                <svg height="36px" viewBox="0 -31 512.00026 512" width="36px"
                                    xmlns="http://www.w3.org/2000/svg">
                                    <path
                                        d="m164.960938 300.003906h.023437c.019531 0 .039063-.003906.058594-.003906h271.957031c6.695312 0 12.582031-4.441406 14.421875-10.878906l60-210c1.292969-4.527344.386719-9.394532-2.445313-13.152344-2.835937-3.757812-7.269531-5.96875-11.976562-5.96875h-366.632812l-10.722657-48.253906c-1.527343-6.863282-7.613281-11.746094-14.644531-11.746094h-90c-8.285156 0-15 6.714844-15 15s6.714844 15 15 15h77.96875c1.898438 8.550781 51.3125 230.917969 54.15625 243.710938-15.941406 6.929687-27.125 22.824218-27.125 41.289062 0 24.8125 20.1875 45 45 45h272c8.285156 0 15-6.714844 15-15s-6.714844-15-15-15h-272c-8.269531 0-15-6.730469-15-15 0-8.257812 6.707031-14.976562 14.960938-14.996094zm312.152343-210.003906-51.429687 180h-248.652344l-40-180zm0 0" />
                                    <path
                                        d="m150 405c0 24.8125 20.1875 45 45 45s45-20.1875 45-45-20.1875-45-45-45-45 20.1875-45 45zm45-15c8.269531 0 15 6.730469 15 15s-6.730469 15-15 15-15-6.730469-15-15 6.730469-15 15-15zm0 0" />
                                    <path
                                        d="m362 405c0 24.8125 20.1875 45 45 45s45-20.1875 45-45-20.1875-45-45-45-45 20.1875-45 45zm45-15c8.269531 0 15 6.730469 15 15s-6.730469 15-15 15-15-6.730469-15-15 6.730469-15 15-15zm0 0" />
                                </svg>
                            </div>
                            
                                <div class="header_delivery_price">
                                    <p>Корзина: руб</p>
                                </div> 
                           
                        </div>
                    </div> -->
                </nav>
            </div>
      </section>
     <section>
       
            <div class="menu-headline">
                <p>Попробуйте неповторимый вкус пиццы на дровах!</p>
            </div>
            <div class="line"></div>
          <div class="pizzas">
              <div class="pizza_row">
                  <cartItem 
                    v-for="product in PRODUCTS"
                    :key="product.id"
                    :product_data="product"
                    @addToCart="addToCart" 
                  />
              </div>
          </div>
           <div class="linetwo"></div>
           <cart 
                v-if="CART.length"
                :cart_data="CART"
           />
     </section>
        <delivery />
       <section>
            <div class="footer">
                <div class="footer_icons">
                    <div><svg height="54" viewBox="0 0 72 72" width="54" xmlns="http://www.w3.org/2000/svg">
                            <g fill="none" fill-rule="evenodd">
                                <path
                                    d="M36,72 L36,72 C55.882251,72 72,55.882251 72,36 L72,36 C72,16.117749 55.882251,-3.65231026e-15 36,0 L36,0 C16.117749,3.65231026e-15 -2.4348735e-15,16.117749 0,36 L0,36 C2.4348735e-15,55.882251 16.117749,72 36,72 Z"
                                    fill="#3E6FA1" />
                                <path
                                    d="M38.8780564,44.394515 C38.9709596,42.9649666 39.6154757,40.7399343 41.2261854,41.9534827 C42.1993467,42.6885795 42.9716048,43.7534827 43.8460564,44.6883214 C44.6996048,45.598773 45.7180564,46.3942569 47.6156048,46.3454827 C48.7408951,46.3164504 51.972766,46.4232892 52.8147015,46.1167085 C55.3590886,45.1934827 50.8509596,40.974515 49.7500564,40.0303859 C49.2867015,39.6332246 48.7676048,39.0676762 48.3704435,38.6472892 C47.8792177,38.1281924 47.6434757,37.6021279 48.0336693,36.7880633 L49.7396048,34.3888375 C50.244766,33.8372246 52.1132822,31.1650956 52.5650241,30.4334827 C53.2153467,29.3790311 54.5496693,27.3061279 52.8297983,26.9739988 C51.8624435,26.7870311 48.7223144,26.9612246 47.5273467,26.9693537 C45.1734112,26.9844504 45.6518628,26.7243214 44.4905725,29.4057408 C43.7171531,31.1894827 41.3295402,35.3933537 40.0637338,35.8729666 C37.716766,36.762515 39.552766,28.2502569 38.5633467,26.7777408 C37.9629596,25.8847085 35.180508,25.9961924 33.8787015,26.0136117 C32.3667015,26.0321924 30.276379,26.1123214 29.8350886,27.3595472 C29.9697983,27.474515 29.8223144,27.3967085 30.0836048,27.5035472 C30.2717338,27.5801924 30.5655402,27.5976117 30.8848951,27.7683214 C31.1682499,27.9181279 31.4260564,28.1817408 31.5735402,28.418644 C32.2865725,29.5590311 32.200637,34.3632892 31.6107015,35.5280633 C30.5063144,37.7043214 27.2802499,31.5901279 26.7274757,30.5008375 C25.9377983,28.9458698 25.6277338,27.4338698 24.7335402,27.0471601 C24.0855402,26.7684504 20.412379,26.9240633 19.4241209,26.9403214 C18.5194757,26.9542569 17.7390886,27.0970956 18.0828306,28.1689666 C18.2558628,28.7089666 18.6669596,29.4696117 18.9154757,30.0142569 C20.4472177,33.3761924 22.8417983,37.5034182 24.9518628,40.2998053 C27.3336693,43.4550311 30.8547015,46.2502569 35.3059273,46.2862569 C38.5029596,46.3118053 38.744508,46.4534827 38.8780564,44.394515"
                                    fill="#FFF" />
                            </g>
                        </svg></div>
                    <div><svg enable-background="new 0 0 24 24" height="54" viewBox="0 0 24 24" width="54"
                            xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
                            <linearGradient id="SVGID_1_" gradientTransform="matrix(0 -1.982 -1.844 0 -132.522 -51.077)"
                                gradientUnits="userSpaceOnUse" x1="-37.106" x2="-26.555" y1="-72.705" y2="-84.047">
                                <stop offset="0" stop-color="#fd5" />
                                <stop offset=".5" stop-color="#ff543e" />
                                <stop offset="1" stop-color="#c837ab" />
                            </linearGradient>
                            <path
                                d="m1.5 1.633c-1.886 1.959-1.5 4.04-1.5 10.362 0 5.25-.916 10.513 3.878 11.752 1.497.385 14.761.385 16.256-.002 1.996-.515 3.62-2.134 3.842-4.957.031-.394.031-13.185-.001-13.587-.236-3.007-2.087-4.74-4.526-5.091-.559-.081-.671-.105-3.539-.11-10.173.005-12.403-.448-14.41 1.633z"
                                fill="url(#SVGID_1_)" />
                            <path
                                d="m11.998 3.139c-3.631 0-7.079-.323-8.396 3.057-.544 1.396-.465 3.209-.465 5.805 0 2.278-.073 4.419.465 5.804 1.314 3.382 4.79 3.058 8.394 3.058 3.477 0 7.062.362 8.395-3.058.545-1.41.465-3.196.465-5.804 0-3.462.191-5.697-1.488-7.375-1.7-1.7-3.999-1.487-7.374-1.487zm-.794 1.597c7.574-.012 8.538-.854 8.006 10.843-.189 4.137-3.339 3.683-7.211 3.683-7.06 0-7.263-.202-7.263-7.265 0-7.145.56-7.257 6.468-7.263zm5.524 1.471c-.587 0-1.063.476-1.063 1.063s.476 1.063 1.063 1.063 1.063-.476 1.063-1.063-.476-1.063-1.063-1.063zm-4.73 1.243c-2.513 0-4.55 2.038-4.55 4.551s2.037 4.55 4.55 4.55 4.549-2.037 4.549-4.55-2.036-4.551-4.549-4.551zm0 1.597c3.905 0 3.91 5.908 0 5.908-3.904 0-3.91-5.908 0-5.908z"
                                fill="#fff" />
                        </svg></div>
                </div>
                <div class="footer_payment">
                    <figure>
                        <img src="../src/assets/images/pay.png">
                    </figure>
                </div>
            </div>
        </section>
    </div>
  </div>
</template>

<script>
import cartItem from './components/cart-item.vue'
import cart from './components/cart.vue'
import {mapActions, mapGetters} from 'vuex'
import Delivery from './components/delivery.vue'

export default {
  name: "App",
  components: {
    cartItem, cart,
    Delivery
  },
  data() {
      return {
      /*  inCart: [] */
  }
},
computed: {
    ...mapGetters([
        'PRODUCTS',
        'CART'
    ])
},
methods: {
    ...mapActions([
        'GET_PRODUCTS_FROM_API',
        'ADD_TO_CART'
    ]),
    addToCart(data) {
        this.ADD_TO_CART(data);
     /*   this.inCart.push(data.name + ' -> ' + data.quantity);
        if(data.quantity > 1) {
         this.inCart.pop();
        }
        console.log(this.inCart);  */
    }
},
mounted() {
    this.GET_PRODUCTS_FROM_API()
    .then((response) => {
        if (response.data) {
            console.log("Data arrived");
        }
    })
 }
}
</script>

<style>
@font-face {
  font-family: "Roboto";
  src: local("Roboto Regular"), local("Roboto-Regular"),
    url("../src/assets/fonts/roboto/Roboto-Regular.ttf") format("ttf");
  font-weight: 400;
  font-style: normal;
}
* {
  margin: 0;
  padding: 0;
  font-family: "Roboto", sans-serif;
}
.image {
    width: 100%;
}
.image_logo {
    width: 100%;
    height: 5%;
}
.content {
  width: 85%;
  border-left: 10px solid black;
  border-right: 10px solid black;
  margin: 0 auto;
}
.header {
    position: relative;
    top: 25px;
}
.header_nav {
    display: flex;
    justify-content: space-around;
    align-items: center;
}
.header_nav_logo {
    width: 20%;
}
.header_nav_logo_container {
    width: 100%;
}
.header_nav_links_container {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.header_nav_link {
    margin: 0 15px 0 15px;
    font-size: 20px;
    color: #000000;
    text-decoration: none;
    border-bottom: 4px solid transparent;
    border-radius: 3px;
    padding-bottom: 6px;
    transition: 0.5s;
}
.header_nav_link:hover {
    border-bottom: 4px solid #5B5B5B;
    transition: 0.5s;
}
.header_delivery_container {
    width: 220px;
    height: 50px;
    background-color: #5B5B5B;
    border-radius: 20px;
    color: white;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
}
.header_delivery_container p {
    transition: 0.5s;
    border-bottom: 3px solid transparent;
}
.header_delivery_container p:hover {
    border-bottom: 3px solid white;
    border-radius: 2px;
    transition: 0.5s;
}
.menu-headline {
    display: flex;
    justify-content: center;
    margin-top: 100px;
    text-align: center;
}
.menu-headline p {
    font-family: 'Prata', serif;
    font-size: 36px;
}
@media screen and (max-width: 1120px) {
    .menu-headline p {
        font-size: 24px;
    }
}
@media screen and (max-width: 810px) {
    .menu-headline p {
        font-size: calc(8px + 16 * (100vw / 1920));
    }
}

/* Hide nav menu */

@media screen and (max-width: 850px) {
    .header_nav_links {
        display: none;
    }
    .header_nav {
        display: flex;
        justify-content: space-around;
        align-items: center;
    }
}
/* Hide burger-menu */
@media screen and (min-width: 851px) {
    .burger-menu {
        display: none;
    }
}

/* Smaller cart */
@media screen and (max-width: 560px) {
    .header_delivery_container{
        width: 120px;
        height: 36px;
    }
    .header_delivery_container p {
        font-size: calc(7px + 16 * (100vw / 1920));
    }
    .header_delivery_container svg {
       height: 24px;
       width: 24px;
    }
    .burger-menu {
        width: 18px;
        height: 18px;
        margin-bottom: 18px;
    }
}
@media screen and (max-width: 300px) {
    .header_delivery_container{
        width: 90px;
    }
}
.line {
    width: 85%;
    height: 10px;
    border-radius: 0 15px 0 15px;
    background-color: black;
    margin: 30px auto 0 auto;
}
.pizzas {
    margin-top: 60px;
}
.pizza_row {
    display: flex;
    flex-direction: row;
    justify-content: center;
    flex-wrap: wrap;
}
.linetwo {
    width: 85%;
    height: 10px;
    border-radius: 15px 0 15px 0;
    background-color: black;
    margin: 30px auto 0 auto;
}
.footer {
    display: flex;
    justify-content: center;
    flex-direction: column;
    background-color: black;
    margin-top: 50px;
    padding-bottom: 40px;
}
.footer_icons {
    display: flex;
    justify-content: space-evenly;
    width: 15%;
    margin: 30px auto 0 auto;
}
.footer_icons svg {
    border-bottom: 3px solid transparent;
    transition: 0.5s;
    padding-bottom: 5px;
}
.footer_icons svg:hover {
    border-bottom: 3px solid white;
    transition: 0.5s;
    border-radius: 3px;
}
.footer_payment {
  width: 70%;
  margin: 30px auto 0 auto;
}
.footer_payment figure img{
  width: 100%;
}
@media screen and (max-width: 1350px) {
    .footer_icons {
        width: 20%;
    }
}
@media screen and (max-width: 850px) {
    .footer_icons {
        width: 30%;
    }
}
@media screen and (max-width: 502px) {
    .footer_icons {
        width: 40%;
    }
}
</style>