<template>
  <section class="Header">

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
      <img src="imgs/desktop_pick_yours.svg">
    </div>
    <div class="Account_Text">
      <img src="imgs/my_account_text.svg">
    </div>
    <div class="Cart_Text">
      <img src="imgs/cart_text.svg">
    </div>
    <div class="wrapper">

      <input type="checkbox" id="navigation" />
      <label for="navigation">
        <img src="imgs/rectangle.svg" alt="Menu" class="Menu">
      </label>

      <nav>

        <ul>
          <img src="imgs/menu_logo.svg">
          <li>
            <a href="">Subscription</a>
          </li>
          <li>
            <a href="">Gifting</a>
          </li>
          <li>
            <a href="">Our Story</a>
          </li>
          <li>
            <a href="">Philosophy</a>
          </li>
          <li>
            <a href="">Home</a>
          </li>
          <li>
            <a href="">Styling</a>
          </li>
          <li>
            <a href="">Care Guide</a>
          </li>
          <li>
            <a href="">My Account</a>
          </li>
        </ul>
      </nav>
    </div>

  </section>
</template>

<script>
export default {
  name: 'Header'
}
</script>
<style>
@font-face {
  font-family: "Leighton Light";
  src: url("/fonts/leighton-light.woff2");
}
.Header {
  display: flex;
  position: fixed;
  justify-content: space-evenly;
  width: 100%
}

.Header_Logo {
  width: 137px;
}

.Header_Cart {
  margin-right: 20px;
  width: 24.44px;
}

.Header_Account {
  width: 20px;
}
.Header_Menu {
  width: 26px;
}

@media screen and (max-width: 427px) {
  .Pick_Yours, .Account_Text, .Cart_Text  {
    display: none;
  }
}

@media screen and (min-width: 426px) {
  .Header_Cart, .Header_Account {
    display: none;
  }
}

@media screen and (min-width: 426px) {
  .Account_Text {

    margin-right: -100px;
  }

  .Cart_Text {

    margin-right: -80px;
  }

  .Pick_Yours {
    margin-top: -30px;
    margin-right: -70px;
  }
  .Header_Logo {
    width: 204px;
    margin-left: 381px;
    margin-right: 50px;

  }
  .Header_Menu {
    margin-left: 0px;

  }
}

body, html{
  height:100%;
}
body{
  padding:0;
  margin:0;
}
p, li{
  font-family:"Leighton Light";
  color:#fff;
  margin:0 0 1em;
}
section li{
  margin:0 0 10px;
}
h1{
  font-size:2.5em;
  font-weight:300;
}
p{
  font-size:1em;
  line-height:1.5em;
}
section{
  padding:30px 30px 30px 80px;
  -moz-transition:all 200ms ease-in;
  -webkit-transition:all 200ms ease-in;
  -o-transition:all 200ms ease-in;
  transition:all 200ms ease-in;

}
nav{
  position:fixed;
  top:0;
  left:0;
  width:250px;
  height:100%;
  margin:0 0 0 -250px;
  -moz-transition:all 200ms ease-in;
  -webkit-transition:all 200ms ease-in;
  -o-transition:all 200ms ease-in;
  transition:all 200ms ease-in;
}
nav ul{
  width:250px;
  height:100%;
  padding:0;
  margin:0;
  list-style:none;
  background:#fff;

}
nav li{
  margin:0;
}
nav a{
  color:#000;
  font-size:1em;
  font-family: "Leighton Light";
  display:block;
  padding:12px 15px;
  letter-spacing:2px;
}

label{
  display:block;
  font-family: "Leighton Light";
  width:42px;
  position:fixed;
  left:60px;
  -moz-transition:all 200ms ease-in;
  -webkit-transition:all 200ms ease-in;
  -o-transition:all 200ms ease-in;
  transition:all 200ms ease-in;
  z-index:500;
}

input[type="checkbox"]:checked ~ nav{
  margin:0;
}
input[type="checkbox"]:checked ~ label{
  left:260px;
}

</style>
