<template>
  <footer>
    <section class="shoplink">
      <div class="container">
        <img
          src="../assets/buy-comics-digital-comics.png"
          alt="Digital Comics"
        />
        <p>DIGITAL COMICS</p>
        <img src="../assets/buy-comics-merchandise.png" alt="Digital Comics" />
        <p>DC MERCHANDISE</p>
        <img
          src="../assets/buy-comics-subscriptions.png"
          alt="Digital Comics"
        />
        <p>SUBSCRIPTION</p>
        <img src="../assets/buy-comics-shop-locator.png" alt="Digital Comics" />
        <p>COMIC SHOP LOCATOR</p>
        <img
          id="powervisa"
          src="../assets/buy-dc-power-visa.svg"
          alt="Digital Comics"
        />
        <p>DC POWER VISA</p>
      </div>
    </section>
    <section class="footernav">
      <div class="container">
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
      </div>
    </section>
    <section class="footersocial">
      <div class="container">
        <a id="signup" href="#">SIGN-UP NOW!</a>
        <div class="social">
          <p>FOLLOW US</p>
          <img src="../assets/footer-facebook.png" alt="facebook" />
          <img src="../assets/footer-twitter.png" alt="facebook" />
          <img src="../assets/footer-youtube.png" alt="facebook" />
          <img src="../assets/footer-pinterest.png" alt="facebook" />
          <img src="../assets/footer-periscope.png" alt="facebook" />
        </div>
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
  padding: 30px 0px;
  .container {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    width: 75%;
    margin: auto;
    img {
      width: 50px;
    }
    p {
      color: white;
      margin: 0px 80px 0px 10px;
    }
  }
}
.footernav {
  background-image: url("../assets/footer-bg.jpg");
  color: white;
  padding: 50px 0px;
  .container {
    display: flex;
    column-gap: 30px;
    width: 80%;
    margin: auto;
    ul {
      list-style-type: none;
      padding: 0;
      a {
        text-decoration: none;
        color: gray;
        &:hover {
          color: white;
        }
      }
    }
  }
}
.footersocial {
  background-color: #303030;
  padding: 50px 0px;
  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 80%;
    margin: auto;
    a {
      color: white;
      text-decoration: none;
      border: 2px solid #0c7cec;
      padding: 10px;
    }
    .social {
      display: flex;
      align-items: center;
      column-gap: 20px;
      p {
        display: inline-block;
        color: #0c7cec;
        font-weight: bold;
      }
    }
  }
}
</style>