<template>
  <HeaderComponent />
  <MainComponent />
  <BlueSectionComponent />
  <FooterComponent />
</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import MainComponent from "./components/MainComponent.vue";
import FooterComponent from "./components/FooterComponent.vue";
import BlueSectionComponent from "./components/BlueSectionComponent.vue";

export default {
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent,
    BlueSectionComponent,
  },
};
</script>

<style lang="scss" scoped></style>
