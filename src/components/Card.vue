<template>
  <div class="card">
    <img :src="Img" :alt="Series" />
    <p>{{ Series }}</p>
  </div>
</template>

<script>
export default {
  name: "CardComponent",
  props: {
    Fumetto: Object,
    Img: String,
    Series: String,
  },
};
</script>

<style lang="scss" scoped>
.card {
  width: calc(100% / 6 - 25px);
  img {
    width: 100%;
  }
}
</style>