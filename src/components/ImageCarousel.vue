<script setup>
import { onMounted } from 'vue'

onMounted(() => {
  const setSlidesPerView = () => {
    const swiperEl = document.querySelector('swiper-container')
    const imageWidth = document.querySelector('.image-carousel-container__image').offsetWidth
    const slidesAvailable = window.innerWidth / imageWidth
    swiperEl.setAttribute('slides-per-view', slidesAvailable)
  }
  window.addEventListener('resize', setSlidesPerView)
  setSlidesPerView()
})
</script>

<template>
  <main class="image-carousel-container">
    <swiper-container
      autoplay-delay="5000"
      spaceBetween="0"
      freemode="true"
      loop="true"
      grabCursor="true"
      cssMode="true"
    >
      <swiper-slide
        ><img src="../assets/random-img.jpg" class="image-carousel-container__image"
      /></swiper-slide>
      <swiper-slide
        ><img src="../assets/random-img-2.jpg" class="image-carousel-container__image"
      /></swiper-slide>
      <swiper-slide
        ><img src="../assets/random-img.jpg" class="image-carousel-container__image"
      /></swiper-slide>
      <swiper-slide
        ><img src="../assets/random-img-2.jpg" class="image-carousel-container__image"
      /></swiper-slide>
      <swiper-slide
        ><img src="../assets/random-img.jpg" class="image-carousel-container__image"
      /></swiper-slide>
      <swiper-slide
        ><img src="../assets/random-img-2.jpg" class="image-carousel-container__image"
      /></swiper-slide>
    </swiper-container>
  </main>
</template>

<style scoped lang="scss">
.image-carousel-container {
  &__image {
    aspect-ratio: 1 / 1;
    width: 600px;
  }
}
</style>
