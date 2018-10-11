<template>
<section class="Hero">
  <div class="Hero__copy">
    <h1>{{ title1 }}</h1>
    <h4>{{ paragraph }}</h4>
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
    flex: column nowrap;
    align-items: center;
    justify-content: center;
    background: url("/imgs/home_hero.jpg") center;
    background-size: cover;
    height: 90vh;
}

.Hero__copy {
  max-width: 250px;
  margin: 0 auto;
  font-family: "Leighton Light";
  text-align: center;
}

</style>
