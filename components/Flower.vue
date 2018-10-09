<template lang="html">
  <div class="Picker">
    <div class="Picker__preview">
      <img v-for="(img, i) in imgs" :key="i" :src="`imgs/home_product_flower_${img}`" alt="" class="Picker__preview__flower">
    </div>
    <div class="Picker__information">i</div>
    <h2 class="Picker__title">SAMPLE THE SEASONS</h2>

    <p class="Picker__text">What would you like:</p>
    <button class="Picker__dropdown__button" type="button" name="button">SUBSCRIPTION</button>

    <p class="Picker__text">How often:</p>
    <button class="Picker__dropdown__button" type="button" name="button">WEEKLY</button>

    <p class="Picker__text">How many varieties of flowers:</p>
    <button class="Picker__dropdown__button" type="button" name="button">1</button>

    <h1 class="Picker__price">£4.00</h1>

    <p class="Picker__text__bottom">per bunch, per week</p>
    <!-- <p class="Picker__text__bottom">week</p> -->

    <button class="Button Picker__subscribe__button"type="button" name="button">SUBSCRIBE</button>

    <p class="Picker__charge__text">Charged every delivery Cancel with just 48 hours</p>

    <p class="Picker__text__Faqs">FAQs</p>

  </div>
</template>

<script>
export default {
  name: "Flower",
  data() {
    return {
      imgs: [
        '1.png',
        '2.png',
        '3.png',
      ]
    }
  }
}
</script>

<style>
@font-face {
  font-family: "Brown";
  font-weight: normal;
  font-style: normal;
  src: url("/fonts/lineto-brown-regularwoff2") format("woff2"),
       url("/fonts/lineto-brown-regularwoff") format("woff");
}

@font-face {
  font-family: "Leighton";
  font-weight: normal;
  font-style: normal;
  src: url("/fonts/leighton-light.woff2") format("woff2"),
       url("/fonts/leighton-light.woff") format("woff");
}

body {
  background-color: #F1EEE5;
  font-family: 'Brown';
  font-weight: normal;
}

.Picker {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.Picker__preview {
  width: 100%;
  margin: auto;
}

.Picker__information {
  display: block;
  margin: 0 auto;
  text-align: center;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 1em;
  color: #D8D8D8;
  font-size: 14px;
  width: 1em;
  height: 1em;
  padding: 5px;
}

.Picker__title {
  display: inline-block;
  text-align: center;
  font-weight: normal;
  color: rgba(0, 0, 0, 0.2);
  border-bottom: 1px solid #979797;
}

.Picker__dropdown__button {
  background-color: #FFFFFF;
  width: 350px;
  border-radius: 50px;
  padding: 10px 0;
  font-size: 11px;
}

.Button.Picker__subscribe__button {
color: #F1EEE5;
background-color: #333333;
padding: 20px 40px;
border-radius: 50px;
}

.Picker__text__bottom {
  width: 15%;
  text-align: center;
  color: #979797;
}

.Picker__text__Faqs {
font-size: 14px;
border-bottom: 1px solid #979797;
}
.Picker__charge__text {
  width: 40%;
  text-align: center;
}

@media(min-width: 800px) {
  .Picker__preview {
    width: 50%;
  }
}

.Picker__preview__flower {
  width: calc(100% / 3);
}

button {
  display: block;
  margin: 0 auto;
}

</style>
