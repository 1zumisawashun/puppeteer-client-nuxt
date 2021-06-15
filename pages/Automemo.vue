<template>
  <div>
    <p>Automemo</p>
    <div v-for="post in posts" :key="post.id">
      <div>{{post.company}}</div>
      <div>{{post.price}}</div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
api:[]
    }
  },
  async asyncData({$axios}) {
  const posts = await $axios.$get('http://localhost:3000/api/paypay/automemo')
  console.log(posts);
  return { posts }
},

}
</script>

<style>

</style>