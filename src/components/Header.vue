<template>
  <header>
    <img id="logo" src="../assets/dc-logo.png" alt="logo header" />
    <ul>
      <li><a href="#">CHARACTERS</a></li>
      <li><a href="#">COMICS</a></li>
      <li><a href="#">MOVIES</a></li>
      <li><a href="#">TV</a></li>
      <li><a href="#">GAMES</a></li>
      <li><a href="#">COLLECTIBLES</a></li>
      <li><a href="#">VIDEOS</a></li>
      <li><a href="#">FANS</a></li>
      <li><a href="#">NEWS</a></li>
      <li><a href="#">SHOP</a></li>
    </ul>
  </header>
</template>

<script>
export default {
  name: "HelloWorld",
};
</script>


<style scoped lang="scss">
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0px 200px;
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
          border-bottom: 2px solid #0c7cec;
        }
      }
    }
  }
}
</style>
