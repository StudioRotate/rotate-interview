<template>
  <div class="Peaker">
    <div class="Peaker__wrapper">
      <div class="Peaker__image">
        <img src="/imgs/home_breakout.png" alt="">
      </div>
      <div class="Peaker__text">
        <h2>Delivered to your door every week, fortnight or month</h2>
        <ul>
          <li>Available for subscription or as a one-off bouquet</li>
          <li>Perfect for gifts (or yourself)</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Peaker'
}
</script>
<style>

  @font-face {
    font-family: "Leighton Light";
    font-weight: 600;
    src: url('/fonts/leighton-light.woff') format('woff');
  }

  @font-face {
    font-family: "Brown";
    font-weight: 400;
    src: url('/fonts/lineto-brown-regular.woff') format('woff');
  }

  .Peaker {
    background-color: #F1EEE5;
    padding: 30px;
  }

  .Peaker__wrapper {
    max-width: 1440px;
    margin-left: auto;
    margin-right: auto;
  }

  @media (min-width: 760px) {
    .Peaker__wrapper {
      display: flex;
    }
  }

  .Peaker__text {
    padding: 40px;
    max-width: 500px;
    align-self: center;
  }

  h2 {
    font-family: "Leighton Light";
    font-size: 28px;
    letter-spacing: 1.6px;
    line-height: 34px;
    margin-bottom: 25px;
  }

  @media (min-width: 760px) {
    h2 {
      font-family: "Leighton Light";
      font-size: 36px;
    }
  }

  li {
    font-family: "Brown";
    font-size: 11px;
    letter-spacing: 2px;
    line-height: 23px;
    text-transform: uppercase;
    list-style: disc;
    list-style-position: inside;
  }

  @media (min-width: 760px) {

  }
</style>
