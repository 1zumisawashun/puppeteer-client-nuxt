<template>
  <div class="card-container" id="sec">
    <ul>
      <li>
        <span class="fa fa-code"></span>
        <p class="title01">Automemo</p>
        <div>{{ post.company }}</div>
        <div>{{ post.price }}</div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  props: {
    post: {
      type: Object,
      required: true,
    },
  },
};
</script>
