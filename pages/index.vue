<template>
  <div>
    <Carousel />
      <div class="Slider">
      <div class="Slider__copy">
        <h1>blah blah</h1>
      </div>
        <swiper :options="swiperOption" ref="mySwiper">
        <div class="Slider__images">
          <swiper-slide> <FirstImage /></swiper-slide>
          <swiper-slide> slide 3</swiper-slide>
          <swiper-slide> slide 2</swiper-slide>
        </div>
        </swiper>
      </div>
  </div>
</template>

<script>
import 'swiper/dist/css/swiper.css'
import { swiper, swiperSlide } from 'vue-awesome-swiper'
import Carousel from '@/components/Carousel.vue'
import FirstImage from '@/components/FirstImage.vue'

export default {
  components: {
    Carousel,
    FirstImage,
    swiper,
    swiperSlide
  }
}
</script>

<style>
.Slider {
  display: flex;
  flex: row nowrap;
  width: 100%;
  height: 30%;
}

.Slider__copy {
  width: 33%;
  height: 50%;
}

.Slider__images {
  width: 66%;
}

.Slider img {
  width: 50%;
}
</style>
