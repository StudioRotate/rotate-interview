<template>
  <div class="Carousel">
    <div class="TopNav">
    <div id="Cart">Cart</div>
    <div id="MyAccount">My Account</div>
    <div id="PickYours">Pick Yours</div>
    <div id="MenuButton">Menu Button</div>
    <div id="LeftButton">Left</div>
    <div id="RightButton">Right</div>
  </div>
  </div>
</template>

<script>
export default {
  name: 'Carousel'
}
</script>

<style>
.Carousel {
  position: relative;
  top: 1em;
}
#Cart {
  background: yellow;
  position: absolute;
  right: 3em;
}

#MyAccount {
  background: yellow;
  position: absolute;
  right: 8em;
}

#PickYours {
  background: yellow;
  position: absolute;
  right: 15em;
}

#MenuButton {
  background: yellow;
  position: absolute;
  left: 1em;
}

#LeftButton {
  background: yellow;
  position: absolute;
  right: 6em;
  top: 5em;
}

#RightButton {
  background: yellow;
  position: absolute;
  right: 3em;
  top: 5em;
}

</style>