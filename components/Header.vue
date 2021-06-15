<template>
  <div class="header-container">
    <nuxt-link to="/" class="item">戻る
    </nuxt-link>
    <div class="link">
      <nuxt-link to="/Automemo" class="item">Automemo</nuxt-link>
      <nuxt-link to="/Meetingowl" class="item">Meetingowl</nuxt-link>
      <nuxt-link to="/Pocketalk" class="item">Pocketalk</nuxt-link>
      </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.header-container {
  height: 100px;
  display: flex;
  background-color: #f1f1f1;
  justify-content: space-between;
}
.link {
  width: 40%;
  display: flex;
  justify-content: space-between;
}
.item {
  width: 100px;
}
</style>