<template>
  <carousel
    :per-page="1"
    :autoplay="true"
    :loop="true"
    :pagination-padding="5"
    :autoplay-timeout="4000"
  >
    <slide> <img src="https://placehold.jp/300x150.png" alt="" /> </slide>
    <slide> <img src="https://placehold.jp/300x150.png" alt="" /> </slide>
    <slide> <img src="https://placehold.jp/300x150.png" alt="" /> </slide>
  </carousel>
</template>

<script>
import Carousel from "vue-carousel/src/Carousel.vue";
import Slide from "vue-carousel/src/Slide.vue";
export default {
  components: {
    Carousel,
    Slide,
  },
};
</script>

<style scoped>
.VueCarousel-slide {
  background: #f1f1f1;
  display: flex;
  align-items: center;
  justify-content: center;
  border-right: 1px solid #fff;
  box-sizing: border-box;
}
</style>