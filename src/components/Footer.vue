<template>
  <footer>
    <!-- shop link -->
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
    <!-- footer nav -->
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
    <!-- social link & signup -->
    <section class="footersocial">
      <div class="container">
        <a id="signup" href="#">SIGN-UP NOW!</a>
        <div class="social">
          <p>FOLLOW US</p>
          <!-- <div :key="index" v-for="(item, index) in social">
            <img :src="'../assets/footer-' + item" alt="facebook" />
          </div> -->
          <img src="../assets/footer-facebook.png" alt="facebook" />
          <img src="../assets/footer-twitter.png" alt="twitter" />
          <img src="../assets/footer-youtube.png" alt="youtube" />
          <img src="../assets/footer-pinterest.png" alt="pinterest" />
          <img src="../assets/footer-periscope.png" alt="periscope" />
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
      social: [
        "facebook.png",
        "twitter.png",
        "youtube.png",
        "pinterest.png",
        "periscope.png",
      ],
      shoplink: [
        {
          name: "DIGITAL COMICS",
          image: "comics-digital-comics.png",
        },
        {
          name: "DC MERCHANDISE",
          image: "comics-merchandise.png",
        },
        {
          name: "SUBSCRIPTION",
          image: "comics-subscriptions.png",
        },
        {
          name: "COMIC SHOP LOCATOR",
          image: "comics-shop-locator.png",
        },
        {
          name: "DC POWER VISA",
          image: "dc-power-visa.svg",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/variables";
.shoplink {
  background-color: $blue-DC;
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
      color: $color-white;
      margin: 0px 80px 0px 10px;
    }
  }
}
.footernav {
  background-image: url("../assets/footer-bg.jpg");
  background-size: cover;
  color: $color-white;
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
          color: $color-white;
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
      color: $color-white;
      text-decoration: none;
      border: 2px solid $blue-DC;
      padding: 10px;
    }
    .social {
      display: flex;
      align-items: center;
      column-gap: 20px;
      p {
        display: inline-block;
        color: $blue-DC;
        font-weight: bold;
      }
    }
  }
}
</style>