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
    <section class="footernav">
      <div class="col">
        <ul>
          <h3>DC COMICS</h3>
          <li><a href="#">Characters</a></li>
          <li><a href="#">Comics</a></li>
          <li><a href="#">Movies</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">Games</a></li>
          <li><a href="#">Videos</a></li>
          <li><a href="#">News</a></li>
        </ul>
        <ul>
          <h3>SHOP</h3>
          <li><a href="#">Shop DC</a></li>
          <li><a href="#">Shop DC Collectibles</a></li>
        </ul>
      </div>
      <div class="col">
        <ul>
          <h3>DC</h3>
          <li><a href="#">Term Of Use</a></li>
          <li><a href="#">Privacy policy (New)</a></li>
          <li><a href="#">Ad Choices</a></li>
          <li><a href="#">Advertising</a></li>
          <li><a href="#">Jobs</a></li>
          <li><a href="#">Subscriptions</a></li>
          <li><a href="#">Talent Workshops</a></li>
          <li><a href="#">CPSC Certificates</a></li>
          <li><a href="#">Ratings</a></li>
          <li><a href="#">Shop Help</a></li>
          <li><a href="#">Contact Us</a></li>
        </ul>
      </div>
      <div class="col">
        <ul>
          <h3>SITES</h3>
          <li><a href="#">DC</a></li>
          <li><a href="#">mad Magazine</a></li>
          <li><a href="#">DC Kids</a></li>
          <li><a href="#">DC Universe</a></li>
          <li><a href="#">DC Power Visa</a></li>
        </ul>
      </div>
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
.footernav {
  background-image: url("../assets/footer-bg.jpg");
  padding: 30px;
  color: white;
  display: flex;
  ul {
    list-style-type: none;
    a {
      text-decoration: none;
      color: gray;
      &:hover {
        color: white;
      }
    }
  }
}
</style>