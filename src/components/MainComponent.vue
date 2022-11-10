<template>
  <section>
    <main>
      <div>Content goes here</div>
    </main>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@use "../assets/styles/partials/variables" as *;
@use "../assets/styles/partials/mixins" as *;
section {
  height: 150px;
  background-color: $maingrey;
  main {
    width: 1170px;

    margin: 0 auto;

    div {
      color: white;
      padding-top: 3rem;
      font-size: 25px;
    }
  }
}
</style>
