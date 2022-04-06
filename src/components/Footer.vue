<template>
  <footer>
    <section class="shoplink">
      <img src="../assets/buy-comics-digital-comics.png" alt="Digital Comics" />
      <p>DIGITAL COMICS</p>
      <img src="../assets/buy-comics-merchandise.png" alt="Digital Comics" />
      <p>DC MERCHANDISE</p>
      <img src="../assets/buy-comics-subscriptions.png" alt="Digital Comics" />
      <p>SUBSCRIPTION</p>
      <img src="../assets/buy-comics-shop-locator.png" alt="Digital Comics" />
      <p>COMIC SHOP LOCATOR</p>
      <img
        id="powervisa"
        src="../assets/buy-dc-power-visa.svg"
        alt="Digital Comics"
      />
      <p>DC POWER VISA</p>
    </section>
  </footer>
</template>

<script>
export default {
  name: "FooterComponent",
};
</script>

<style lang="scss" scoped>
.shoplink {
  background-color: #0c7cec;
  padding: 80px 0px 80px 120px;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  #powervisa {
    width: 150px;
  }
  p {
    color: white;
    margin: 0px 80px 0px 10px;
  }
}
</style>