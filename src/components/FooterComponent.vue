<template>
  <section class="upper-footer jumbo-footer">
    <div class="container my-container">
      <div class="lists">
        <div class="up-list">
          <div>
            <div>
              <h3 class="list-title">dc comics</h3>
              <ul>
                <li v-for="(dcomics, index) in dcomics" key="index">
                  <a href="">{{ dcomics.text }}</a>
                </li>
              </ul>
            </div>

            <div class="shop">
              <h3 class="shop-title">shop</h3>
              <ul>
                <li v-for="(shop, index) in shop" key="index">
                  <a href="">{{ shop.text }}</a>
                </li>
              </ul>
            </div>
          </div>

          <div>
            <h3 class="list-title">dc</h3>
            <ul>
              <li v-for="(dc, index) in dc" key="index">
                <a href="">{{ dc.text }}</a>
              </li>
            </ul>
          </div>

          <div>
            <h3 class="list-title">sites</h3>
            <ul>
              <li v-for="(sites, index) in sites" key="index">
                <a href="">{{ sites.text }}</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section class="lower-footer">
    <div class="internal">
      <button class="my-btn">sign-up now!</button>
      <div class="follow">follow us</div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      dcomics: [
        {
          text: "Characters",
          url: "#",
        },
        {
          text: "Comics",
          url: "#",
        },
        {
          text: "Movies",
          url: "#",
        },
        {
          text: "Tv",
          url: "#",
        },
        {
          text: "Games",
          url: "#",
        },
        {
          text: "Videos",
          url: "#",
        },
        {
          text: "News",
          url: "#",
        },
      ],

      shop: [
        {
          text: "Shop DC",
          url: "#",
        },
        {
          text: "Shop DC Collectibles",
          url: "#",
        },
      ],

      dc: [
        {
          text: "Terms of Use",
          url: "#",
        },
        {
          text: "Privacy policy (new)",
          url: "#",
        },
        {
          text: "Ad Choices",
          url: "#",
        },
        {
          text: "Advertising",
          url: "#",
        },
        {
          text: "Jobs",
          url: "#",
        },
        {
          text: "Subscriptions",
          url: "#",
        },
        {
          text: "Talent Workshops",
          url: "#",
        },
        {
          text: "CPSC Certificates",
          url: "#",
        },
        {
          text: "Ratings",
          url: "#",
        },
        {
          text: "Shop Help",
          url: "#",
        },
        {
          text: "Contact Us",
          url: "#",
        },
      ],
      sites: [
        {
          text: "DC",
          url: "#",
        },
        {
          text: "MAD Magazine",
          url: "#",
        },
        {
          text: "DC Kids",
          url: "#",
        },
        {
          text: "DC Universe",
          url: "#",
        },
        {
          text: "DC Power Vista",
          url: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@use "../assets/styles/partials/variables" as *;
@use "../assets/styles/partials/mixins" as *;

.jumbo-footer {
  background-image: url(../assets/img/footer-bg.jpg);
  width: 100%;
  height: 400px;
}
.my-container {
  width: 1170px;
  margin-left: 18rem;
}
.up-list {
  display: flex;
  flex-wrap: wrap;
}

.lists {
  width: 1170px;
  margin: 0 auto;
  div {
    padding: 0 1rem;
  }

  .list-title {
    text-transform: uppercase;
    color: white;
    padding-top: 2rem;
    padding-bottom: 1rem;
  }
  .shop-title {
    color: white;
    text-transform: uppercase;
    margin-bottom: 1rem;
    margin-top: 1rem;
  }
  ul {
    list-style-type: none;
    li {
      a {
        color: $greytext;
        text-decoration: none;
        font-size: 14px;
      }
    }
  }
}

.lower-footer {
  height: 150px;
  background-color: $darkgrey;
  .internal {
    @include dflex;
    max-width: 1170px;
    margin: 0 auto;
  }
  .my-btn {
    padding: 0.8rem 1rem;
    margin-top: 3rem;
    background-color: transparent;
    color: white;
    border: 1px solid $blue;
    font-size: 15px;
    text-transform: uppercase;
    display: inline-block;
  }

  .follow {
    font-size: 20px;
    text-transform: uppercase;
    font-weight: 600;

    color: $blue;
    display: inline-block;

    padding-top: 4rem;
  }
}
</style>
