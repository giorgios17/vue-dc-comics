<template>
  <main>
    <div class="content">--&gt; Content goes here &lt;--</div>
  </main>
</template>

<script>
export default {
  name: "MainComponent",
};
</script>

<style lang="scss" scoped>
main {
  background-color: black;
  color: white;
  .content {
    width: 80%;
    margin: auto;
    padding: 50px;
  }
}
</style>