<template>
<section class="Hero">
  <div class="Hero__copy">
    <h1>The Seasons delivered</h1>
    <p>We source fresh, beautiful and seasonal flowers, and deliver them to your home.</p>
  </div>
</section>
</template>

<script>
export default {
name: 'Hero'
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
  max-width: 400px;
  margin: 0 auto;
  font-family: "Leighton Light";
}
</style>
