<template lang="html">
  <div class="Picker">
    <div class="Picker__preview">
      <img v-for="(img, i) in imgs" :key="i" :src="`imgs/home_product_flower_${img}`" alt="" class="Picker__preview__flower">
    </div>
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

body {
  background-color: #F1EEE5;
}

.Picker__preview {
  width: 100%;
  margin: auto;
}

@media(min-width: 800px) {
  .Picker__preview {
    width: 50%;
  }
}

.Picker__preview__flower {
  width: calc(100% / 3);
}
</style>
