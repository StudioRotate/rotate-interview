<template>
<section class="Header">
<div class="Header_Menu">
  <img src="imgs/rectangle.svg" alt="Menu" class="Menu">
</div>
  <div class="Header_Logo">
  <img src="imgs/logo-large.svg" alt="Logo" class="Logo">
  </div>
  <div class="Header_Account">
    <img src="imgs/account.svg">
</div>
<div class="Header_Cart">
  <img src="imgs/cart.svg" alt="Cart" class="Cart">
</div>
<div class="Pick_Yours">
  <img src="imgs/hero_button.svg">
</div>
<div class="Account_Text">
  <img src="imgs/my_account_text.svg">
</div>
<div class="Cart_Text">
  <img src="imgs/cart_text.svg">
</div>

</section>
</template>

<script>
export default {
name: 'Header'
}
</script>
<style>
  .Header {
    display: flex;
    position: fixed;
    justify-content: flex-end;
    width: 100%;
    margin-top: 20px;

  }

  .Header_Logo {
    width: 137px;
    padding-right: 30px;

  }

  .Header_Cart {
    width: 24.44px;
    padding-right: 30px;
  }

  .Header_Account {
    width: 20px;
    padding-left: 40px;
    padding-right: 20px
  }
  .Header_Menu {
    width: 20%;
    padding-left: 40px;
    padding-right: 45px
  }
@media screen and (max-width: 401px) {
    .Pick_Yours, .Account_Text, .Cart_Text  {
    display: none;
    }
}

@media screen and (min-width: 400px) {
  .Header_Cart, .Header_Account {
    display: none;
  }
}
@media screen and (min-width: 400px) {
.Account_Text {
  width: 20%;
  display: inline-block;
}

.Cart_Text {
  width: 20%;
  display: inline-block;
}
.Pick_Yours {
  width: 20%;
  display: inline-block;
}
.Header_Logo {
  width: 20%;
  display: inline-block;
}
}
</style>
