<template lang="html">
  <div class="Container">
  <div class="Picker">
    <div class="Picker__preview">
      <img v-for="(img, i) in imgs" :key="i" :src="`imgs/home_product_flower_${img}`" alt="" class="Picker__preview__flower">
    </div>
    <div class="Picker__information">i</div>

    <h2 class="Picker__title">SAMPLE THE SEASONS</h2>

<div class="Picker__menu">
    <p class="Picker__text">What would you like:</p>
    <Dropdown :values="values.type"/>

    <button :class="{'Picker__button Picker__button__inactive': activeType !== 1, 'Picker__button': activeType === 1}" name="button" @click="setType(1)">SUBSCRIPTION</button>
    <button :class="{'Picker__button Picker__button__inactive': activeType !== 2, 'Picker__button': activeType === 2}" name="button" @click="setType(2)">GIFTING</button>

    <p class="Picker__text">How often:</p>
    <Dropdown :values="values.regularity"/>

    <button :class="{'Picker__button Picker__button__inactive': activeRegularity !== 1, 'Picker__button': activeRegularity === 1}" name="button" @click="setRegularity(1)">WEEKLY</button>
    <button :class="{'Picker__button Picker__button__inactive': activeRegularity !== 2, 'Picker__button': activeRegularity === 2}" name="button" @click="setRegularity(2)">FORTNIGHTLY</button>
    <button :class="{'Picker__button Picker__button__inactive': activeRegularity !== 3, 'Picker__button': activeRegularity === 3}" name="button" @click="setRegularity(3)">MONTHLY</button>

    <p class="Picker__text">How many varieties of flowers:</p>
    <Dropdown :values="values.quantity"/>

    <button :class="{'Picker__button Picker__button__inactive': activeQuantity !== 1, 'Picker__button Picker__button__quantity': activeQuantity === 1}" name="button" @click="setQuantity(1)">1</button>
    <button :class="{'Picker__button Picker__button__inactive': activeQuantity !== 2, 'Picker__button Picker__button__quantity': activeQuantity === 2}" name="button" @click="setQuantity(2)">3</button>
  </div>

<div class="Picker__price__menu">

    <div class="Picker__price">
      <div class="Picker__price__£">£</div>
      <p class="Picker__price__pounds">{{pounds}}</p>
      <p class="Picker__price__point">.</p>
      <p class="Picker__price__pence">{{pence}}</p>
    </div>

    <p class="Picker__price__text">per bunch, per week</p>

    <button class="Picker__subscribe__button"type="button" name="button">SUBSCRIBE</button>

    <p class="Picker__charge__text">Charged every delivery Cancel with just 48 hours notice</p>
  </div>
</div>

  <div class="Picker__text__faqs__wrapper">
    <div class="Picker__text__faqs">FAQs</div>
  </div>
</div>
</template>

<script>
import Dropdown from './Dropdown'

export default {
  name: "Flower",
  components: {
    Dropdown
  },
  data() {
    return {
      values: {
        type: ['SUBSCRIPTION', 'GIFTING'],
        regularity: ['WEEKLY', 'FORTNIGHTLY', 'MONTHLY'],
        quantity: ['1', '3']
      },
      imgs: [
        '1.png',
        '2.png',
        '3.png',
      ],
      pounds: '40',
      pence: '00',
      activeType: 1,
      activeRegularity: 1,
      activeQuantity: 1
    }
  },
  methods: {
    setType(id) {
      this.activeType = id;
    },
    setRegularity(id) {
      this.activeRegularity = id;
    },
    setQuantity(id) {
      this.activeQuantity = id;
    }
  },
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
  font-family: "Brown";
  /* font should be 'leighton-light' but not renedering */
  font-weight: normal;
  height: 100vh;
}

.Picker__button {
  display: none;
}

.Picker {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.Picker__preview__flower {
  width: calc(100% / 3);
}

.Picker__preview {
  width: 100%;
  margin: auto;
}

.Picker__information {
  text-align: center;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 1em;
  color: #333333;
  font-size: 14px;
  width: 1em;
  height: 1em;
  padding: 5px;
  margin-top: 42px;
}

.Picker__title {
  margin-top: 45px;
  margin-bottom: 51px;
  font-weight: normal;
  color: rgba(0, 0, 0, 0.2);
  border-bottom: 1px solid #979797;
  font-size: 11px;
  padding-bottom: 5px;
}

.Picker__text {
  font-size: 14;
  padding-bottom: 12px;
  padding-top: 24px;
  text-align: center;
}

.Picker__button__inactive {
  display: none;
}

.rotate90 {
  transform: rotate(90deg);
  width: 8px;
}

.Picker__price {
  display: flex;
  font-size: 21px;
  padding-top: 50px;
}

.Picker__price__£,
.Picker__price__pence {
  padding-top: 10px;
}

.Picker__price__pounds {
  font-size: 48px;
}

.Picker__price__point {
  padding-top: 4px;
}

.Picker__subscribe__button {
  font-size: 11px;
  color: #F1EEE5;
  background-color: #333333;
  padding: 15px 40px;
  border-radius: 50px;
  box-shadow: 0px 6px 4px rgba(0, 0, 0, 0.1);
  margin-top: 10px;
}

.Picker__price__text {
  width: 25%;
  text-align: center;
  color: #979797;
  font-size: 12px;
}

.Picker__text__faqs__wrapper {
  text-align: center;
}

.Picker__text__faqs {
  font-size: 14px;
  padding-bottom: 5px;
  border-bottom: 1px solid #979797;
  padding-top: 31px;
  margin-bottom: 110px;
  display: inline-block;
}

.Picker__charge__text {
  width: 40%;
  text-align: center;
  color: #979797;
  font-size: 12px;
  padding-top: 31px;
}

.Picker__price__menu {
  display: flex;
  flex-direction: column;
  align-items: center;
}

@media(min-width: 800px) {
  .Picker__preview {
    width: 50%;
  }

  .Picker {
    flex-direction: row;
    position: relative;
    padding-top: 50px;
  }

  .Picker__menu {
    flex-direction: column;
    order: -1;
    padding-left: 80px;
  }

  .Picker__text {
    text-align: left;
  }

  .Picker__text__faqs__wrapper {
    text-align: left;
    padding-left: 60px;
  }

  .Picker__button {
    display: inline-block;
    background-color: #FFFFFF;
    width: 330px;
    border-radius: 50px;
    padding: 17px 0;
    font-size: 11px;
    width: auto;
    padding: 17px;
  }

  .Picker__button__inactive {
    display: inline-block;
    background-color: #F1EEE5;
    color: rgba(51, 51, 51, 0.35)
  }

  .Picker__button__quantity {
    width: 1em;
    height: 1em;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .Picker__information {
    position: absolute;
    bottom: -10px;
    left: 50%;
  }

  .Picker__charge__text {
    width: 50%;
  }

  .Picker__title {
    position: absolute;
    bottom: -100px;
    left: 47%;
  }

  .Dropdown__button {
    display: none;
  }
}
</style>
