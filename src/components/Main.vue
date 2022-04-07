<template>
  <main>
    <div class="jumbotron">
      <span class="current-series">CURRENT SERIES</span>
    </div>
    <div class="content">
      <!-- <div class="card" :key="index" v-for="(fumetto, index) in Fumetto">
        <img :src="fumetto.thumb" :alt="fumetto.series" />
        <p>{{ fumetto.series }}</p>
      </div> -->
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
main {
  background-color: black;
  color: white;
  .jumbotron {
    background-image: url("../assets/jumbotron.jpg");
    height: 400px;
    position: relative;
    .current-series {
      background-color: #0c7cec;
      padding: 10px 25px;
      font-size: 18px;
      color: white;
      position: absolute;
      bottom: -20px;
      left: 150px;
    }
  }
  .content {
    display: flex;
    flex-wrap: wrap;
    column-gap: 25px;
    width: 80%;
    margin: auto;
    padding: 50px;
  }
  .text-center {
    text-align: center;
    #loadMore {
      text-align: center;
      background-color: #0c7cec;
      border: 0;
      color: white;
      padding: 10px 40px;
      cursor: pointer;
      margin-bottom: 20px;
    }
  }
}
</style>