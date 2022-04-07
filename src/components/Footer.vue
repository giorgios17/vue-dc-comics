<template>
  <footer>
    <!-- shop link -->
    <section class="infolink">
      <div class="container">
        <div class="info" :key="index" v-for="(link, index) in infolink">
          <img :src="link.image" :alt="link.name" />
          <p>{{ link.name }}</p>
        </div>
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
          <div :key="index" v-for="(social, index) in allSocial">
            <img :src="social" alt="social" />
          </div>
          <!-- <img src="../assets/footer-facebook.png" alt="facebook" />
          <img src="../assets/footer-twitter.png" alt="twitter" />
          <img src="../assets/footer-youtube.png" alt="youtube" />
          <img src="../assets/footer-pinterest.png" alt="pinterest" />
          <img src="../assets/footer-periscope.png" alt="periscope" /> -->
        </div>
      </div>
    </section>
  </footer>
</template>

<script>
import Comic from "@/assets/buy-comics-digital-comics.png";
import Merchandise from "@/assets/buy-comics-merchandise.png";
import ShopLocator from "@/assets/buy-comics-shop-locator.png";
import Subscriptions from "@/assets/buy-comics-subscriptions.png";
import PowerVisa from "@/assets/buy-dc-power-visa.svg";
import Periscope from "@/assets/footer-periscope.png";
import Pinterest from "@/assets/footer-pinterest.png";
import Facebook from "@/assets/footer-facebook.png";
import Twitter from "@/assets/footer-twitter.png";
import Youtube from "@/assets/footer-youtube.png";

export default {
  name: "FooterComponent",
  data: function () {
    return {
      //FOOTER NAV DCCOMICS
      dcComics: [
        "Characters",
        "Comics",
        "Movies",
        "TV",
        "Games",
        "Videos",
        "News",
      ],
      //FOOTER NAV SHOP
      shop: ["Shop DC", "Shop DC Collectibles"],
      //FOOTER NAV DC
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
      //FOOTER NAV SITES
      sites: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"],
      // SOCIAL
      allSocial: [Facebook, Twitter, Youtube, Pinterest, Periscope],
      //INFOLINK
      infolink: [
        {
          name: "DIGITAL COMICS",
          image: Comic,
        },
        {
          name: "DC MERCHANDISE",
          image: Merchandise,
        },
        {
          name: "SUBSCRIPTION",
          image: Subscriptions,
        },
        {
          name: "COMIC SHOP LOCATOR",
          image: ShopLocator,
        },
        {
          name: "DC POWER VISA",
          image: PowerVisa,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/style/variables";
.infolink {
  background-color: $blue-DC;
  padding: 30px 0px;
  .info {
    display: flex;
    align-items: center;
  }
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
.prova {
  display: flex;
}
</style>