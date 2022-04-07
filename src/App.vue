<template>
  <div id="app">
    <Header />
    <Main :Fumetto="Fumetto" />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";
import Fumetto from "./assets/data/dc-comics";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
  data() {
    return {
      Fumetto,
    };
  },
};
</script>

<style lang="scss">
@import "@/assets/style/variables";
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
