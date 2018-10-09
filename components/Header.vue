<template>
<section class="Header">
  <div class="Header_Wrapper">
  <img src="imgs/logo-large.svg" alt="Logo" class="Logo">
  </div>
  <div class="Header_Account">
    <img src="imgs/account.svg">
</div>
<div class="Header_Cart">
  <img src="imgs/cart.svg" alt="Cart" class="Cart">
</div>
<div class="Header_Menu">
  <img src="" >
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
    padding-top: 25px;
    padding-right: 30px;
    padding-bottom: 50px;
    padding-left: 30px;
  }

  .Header_Wrapper {
    width: 137px;
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
    width: 20px;
    padding-left: 40px;
    padding-right: 20px
  }


</style>
