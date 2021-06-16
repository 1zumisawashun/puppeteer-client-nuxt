<template>
  <div>
    <Carousel></Carousel>
    <div class="post-wrapper">
      <div v-for="post in posts" :key="post.id">
        <Card :post="post"></Card>
      </div>
    </div>
  </div>
</template>

<script>
import Carousel from "@/components/Carousel.vue";
import Card from "@/components/Card.vue";
export default {
  components: {
    Carousel,
    Card,
  },
  data() {
    return {
      api: [],
    };
  },
  async asyncData({ $axios }) {
    const posts = await $axios.$get(
      "http://localhost:3000/api/paypay/automemo"
    );
    console.log(posts);
    return { posts };
  },
};
</script>

<style scoped>
.post-wrapper {
  width: 80%;
  margin: 0 auto;
  display: flex;
  flex-wrap: wrap;
}
</style>