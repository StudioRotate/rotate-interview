<template>
<section class="Hero">
  <div class="Hero__copy">
    <h1>{{ title1 }}</h1>
    <h4>{{ paragraph }}</h4>
  <div class="Hero_button">
    <img src="imgs/hero_button.svg" alt="Home_Button" class="Home_button">
  </div>
  </div>
</section>
</template>

<script>
export default {
name: 'Hero',
data() {
  return {
    title1: 'The Seasons, delivered',
    paragraph: 'We source fresh, beautiful and seasonal flowers, and deliver them to your home.'
  }
}
}
</script>

<style>
@font-face {
    font-family: "Leighton Light";
    src: url("/fonts/leighton-light.woff2");
}
.Hero {
    display: flex;
    align-items: center;
    justify-content: center;
    background: center;
    background-image: url(/imgs/home_hero.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    height: 90vh;
}

@media screen and (min-width: 401px) {
    .Hero {
    background-image: url(/imgs/hero_background_desktop.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    }
}

.Hero__copy {
  max-width: 250px;
  margin: 0 auto;
  font-family: "Leighton Light";
  text-align: center;
}

.Hero_button {
  padding-top: 30px;
}


</style>
