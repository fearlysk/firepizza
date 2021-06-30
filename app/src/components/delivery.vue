<template>
    <div id="delivery">
          <section>
    <div class="delivery">
        <div class="delivery-headline">
            <p>Доставка</p>
        </div>

        <div class="delivery-content">
            <h1>Чтобы оформить Ваш заказ, заполните форму</h1>

                <div class="delivery-content-form">
                    <form>
                        <p>Имя: *</p>
                           <input type="text" name="name" />
                        <p>Контактный телефон: *</p>
                           <input type="number" name="phonenumber" />
                        <p>Время получения заказа: *</p>
                           <div class="hrsmins">
                               <input id="hrs" type="number" name="hrs" placeholder="Часы">
                               <input id="mins" type="number" name="mins" placeholder="Минуты">
                           </div>
                    </form>
            <div class="delivery-content-form-minsk">
                <form>
                    <h1>Адрес доставки в Минске</h1>
                    <p>Улица: *</p>
                    <input type="text" name="street" />
                        <div class="delivery-content-form-minsk-homeaddress">
                          <div>
                            <p>Номер дома: *</p>
                            <input type="number" name="homenumber" />
                          </div>
                          <div class="l">
                            <p>Номер корпуса:</p>
                            <input type="number" name="housing" />
                           </div>
                           <div class="l">
                            <p>Номер квартиры:</p>
                            <input type="number" name="flatnumber" />
                           </div>
                        </div>
                        <h2 class="delivery-content-form-minsk-homeaddress-note">Примечание (подъезд, этаж, доп. номер телефона):</h2>
                        <textarea rows="10" cols="30" name="note" style="padding: 10px; margin-top: 10px"></textarea>
                        <input type="submit" name="ordersubmit" value="Подтвердить заказ">
                    </form>
                 </div>    
                </div>
               </div>
        </div>
   </section> 

</div> 
</template>

<script>
export default {
    name: 'delivery',
    components: {},
    data() {
        return {}
    }
}
</script>

<style>
.cart-headline {
    display: flex;
    justify-content: center;
    margin-top: 100px;
    text-align: center;
}
.cart-headline p {
    font-family: 'Prata', serif;
    font-size: calc(22px + 16 * (100vw / 1920));
    padding-bottom: 6px;
    border-bottom: 3px solid black;
}
.cart-content {
    margin: 60px 0 0 20%;
}
.cart-content p {
    font-family: 'Prata', serif;
    font-size: calc(12px + 16 * (100vw / 1920));
}
.cart-footer {
    display: flex;
    margin-top: 60px;
    justify-content: center;
}
.cart-footer button {
    padding: 7px 35px 7px 35px;
    color: white;
    background-color: black;
    font-size: 20px;
    border-radius: 4px;
    font-family: 'Prata', serif;
}
.delivery-headline {
    display: flex;
    justify-content: center;
    margin-top: 100px;
    text-align: center;
}
.delivery-headline p {
    font-family: 'Prata', serif;
    font-size: calc(22px + 16 * (100vw / 1920));
    padding-bottom: 6px;
    border-bottom: 3px solid black;
}
.delivery-content {
    margin: 30px auto 0 auto;
    width: 85%;
    text-align: center;
    font-family: 'Prata', serif;
}
.delivery-content h1 {
    font-family: 'Prata', serif;
    font-size: calc(22px + 16 * (100vw / 1920));
    padding-bottom: 6px;
    border-bottom: 3px solid black;
    width: 80%;
    margin: 0 auto;
}
.delivery-content-form form {
    margin-top: 40px;
    display: flex;
    flex-direction: column;
    margin-left: 10%;
    padding-bottom: 50px;
    border-bottom: 3px solid black;
}
.delivery-content-form p {
    text-align: left;
    font-size: calc(17px + 16 * (100vw / 1920));
    margin-top: 15px;
}
input {
    margin-top: 15px;
    width: 70%;
    float: left;
    height: 33px;
    border: 1px solid black;
    border-radius: 4px;
}
.hrsmins {
    display: flex;
    flex-direction: row;
    justify-content: left;
    width: 50%;
}
.hrsmins input {
    width: 50%;
}
#mins {
    margin-left: 5%;
}
input::placeholder {
    text-align: center;
}
.delivery-content-form-minsk h1 {
    width: 50%;
}
.delivery-content-form-minsk-homeaddress {
    display: flex;
}
.l {
    margin-left: 10%;
}
.delivery-content-form-minsk-homeaddress input {
    width: 100%;
} 
@media screen and (max-width: 500px) {
    .delivery-content-form-minsk-homeaddress {
        display: block;
    }
    .l {
        margin-top: 70px;
    }
    input[type="submit"] {
        width: 100% !important;
    }
}
.delivery-content-form-minsk-homeaddress-note {
    width: 90%;
    text-align: left;
    margin-top: 30px;
}
input[type="submit"] {
    margin: 30px auto 0 auto;
    font-size: 20px;
    width: 60%;
    color: white;
    background-color: black;
    font-family: 'Prata', serif;
}
</style>