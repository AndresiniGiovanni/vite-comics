<template>
  <section>
    <div class="d-flex align-items-center my-cont">
      <div class="info" v-for="(img, index) in bluSection">
        <img :src="img.img" alt="" />
        <span>{{ img.text }}</span>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      bluSection: [
        {
          img: "/public/img/buy-comics-digital-comics.png",
          text: "digital comics",
        },
        {
          img: "/public/img/buy-comics-merchandise.png",
          text: "dc merchandise",
        },
        {
          img: "/public/img/buy-comics-subscriptions.png",
          text: "subscription",
        },
        {
          img: "/public/img/buy-comics-shop-locator.png",
          text: "comic shop locator",
        },
        {
          img: "/public/img/buy-dc-power-visa.svg",
          text: "dc power visa",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@use "../assets/styles/partials/variables" as *;
@use "../assets/styles/partials/mixins" as *;
.my-cont {
  max-width: 1170px;
  margin: 0 auto;
  .info {
    margin-top: 2.7rem;
  }
  span {
    text-transform: uppercase;
    color: white;
    font-size: 13px;
    margin-left: 1rem;
    margin-right: 1.5rem;
  }
}
section {
  width: 100%;
  height: 120px;
  background-color: $blueSection;
  img {
    width: 15%;
  }
}
</style>
