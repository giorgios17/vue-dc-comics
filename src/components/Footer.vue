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
            <li :key="index" v-for="(link, index) in dcComics">
              <a href="#">{{ link }}</a>
            </li>
          </ul>
          <ul>
            <h3>SHOP</h3>
            <li :key="index" v-for="(link, index) in shop">
              <a href="#">{{ link }}</a>
            </li>
          </ul>
        </div>
        <div class="col">
          <ul>
            <h3>DC</h3>
            <li :key="index" v-for="(link, index) in dc">
              <a href="#">{{ link }}</a>
            </li>
          </ul>
        </div>
        <div class="col">
          <ul>
            <h3>SITES</h3>
            <li :key="index" v-for="(link, index) in sites">
              <a href="#">{{ link }}</a>
            </li>
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
  data: function () {
    return {
      dcComics: [
        "Characters",
        "Comics",
        "Movies",
        "TV",
        "Games",
        "Videos",
        "News",
      ],
      shop: ["Shop DC", "Shop DC Collectibles"],
      dc: [
        "Terms of Use",
        "Privacy Policy (New)",
        "Ad Choices",
        "Advertising",
        "Jobs",
        "Subscriptions",
        "Talent Workshops",
        "CPSC Certificates",
        "Ratings",
        "Shop Help",
        "Contact Us",
      ],
      sites: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"],
    };
  },
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
  background-size: cover;
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
  padding: 30px 0px;
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