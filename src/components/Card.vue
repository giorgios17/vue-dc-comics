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
  width: calc(100% / 6);
  margin-bottom: 15px;
  img {
    width: 150px;
    height: 150px;
    object-fit: cover;
    object-position: 0% 0%;
  }
}
</style>