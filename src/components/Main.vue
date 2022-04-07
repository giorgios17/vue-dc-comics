<template>
  <main>
    <div class="jumbotron">
      <span class="current-series">CURRENT SERIES</span>
    </div>
    <div class="content">
      <CardComponent
        v-for="(fumetto, index) in Fumetto"
        :key="'fumetto' + index"
        :Img="fumetto.thumb"
        :Series="fumetto.series"
      />
    </div>
    <div class="text-center">
      <button id="loadMore">LOAD MORE</button>
    </div>
  </main>
</template>

<script>
import CardComponent from "@/components/Card.vue";

export default {
  name: "MainComponent",
  props: {
    Fumetto: Array,
  },
  components: {
    CardComponent,
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/variables";
main {
  background-color: black;
  color: $color-white;
  .jumbotron {
    background-image: url("../assets/jumbotron.jpg");
    height: 400px;
    position: relative;
    .current-series {
      background-color: $blue-DC;
      padding: 10px 25px;
      font-size: 18px;
      color: $color-white;
      position: absolute;
      bottom: -20px;
      left: 250px;
    }
  }
  .content {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    width: 70%;
    margin: auto;
    padding: 50px;
  }
  .text-center {
    text-align: center;
    #loadMore {
      text-align: center;
      background-color: $blue-DC;
      border: 0;
      color: $color-white;
      padding: 10px 40px;
      cursor: pointer;
      margin-bottom: 20px;
    }
  }
}
</style>