<template>
  <header>
    <div>
      <img src="../assets/img/dc-logo.png" alt="" />
    </div>
    <nav>
      <ul>
        <li v-for="(nav, index) in nav" key="index">
          <a href="nav.url" :class="{ active: nav.current }">{{ nav.text }}</a>
        </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  data() {
    return {
      nav: [
        {
          text: "characters",
          url: "#",
          current: false,
        },
        {
          text: "comics",
          url: "#",
          current: true,
        },
        {
          text: "movies",
          url: "#",
          current: false,
        },
        {
          text: "tv",
          url: "#",
          current: false,
        },
        {
          text: "games",
          url: "#",
          current: false,
        },
        {
          text: "collectibles",
          url: "#",
          current: false,
        },
        {
          text: "videos",
          url: "#",
          current: false,
        },
        {
          text: "fans",
          url: "#",
          current: false,
        },
        {
          text: "news",
          url: "#",
          current: false,
        },
        {
          text: "shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
@use "../assets/styles/partials/variables" as *;
@use "../assets/styles/partials/mixins" as *;

header {
  max-width: 1170px;
  height: 150px;
  margin: 0 auto;
  @include dflex;

  img {
    padding-top: 1rem;
  }

  ul {
    list-style: none;
    margin-top: 3rem;

    li,
    a {
      display: inline-block;
      padding: 0.4rem;
      text-decoration: none;
      font-weight: 600;
      color: $blacktext;
      text-transform: uppercase;

      &.active,
      &.hover {
        background: $lightblue;
      }
    }
  }
}
</style>
