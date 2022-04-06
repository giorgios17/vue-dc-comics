<template>
  <header>
    <img id="logo" src="../assets/dc-logo.png" alt="logo header" />
    <ul>
      <li :key="index" v-for="(item, index) in navHeader">
        <a href="#">{{ item }}</a>
      </li>
    </ul>
  </header>
</template>

<script>
export default {
  name: "HeaderComponent",
  data: function () {
    return {
      navHeader: [
        "CHARACTERS",
        "COMICS",
        "MOVIES",
        "TV",
        "GAMES",
        "COLLECTIBLES",
        "VIDEOS",
        "FANS",
        "NEWS",
        "SHOP",
      ],
    };
  },
};
</script>


<style scoped lang="scss">
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 30px 0px;
  width: 80%;
  margin: auto;
  ul {
    list-style-type: none;
    padding: 0;
    li {
      display: inline-block;
      margin: 0 10px;
      a {
        color: black;
        text-decoration: none;
        padding-bottom: 40px;
        &:hover {
          color: #0c7cec;
          border-bottom: 5px solid #0c7cec;
        }
      }
    }
  }
}
</style>
