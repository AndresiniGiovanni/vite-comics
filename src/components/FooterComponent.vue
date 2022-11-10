<template>
  <section class="upper-footer">
  <div class="jumbo-footer">
  </div>
  </section>

  <section class="lower-footer">
    <div class="internal">
      <button class="my-btn">sign-up now!</button>
      <div class="follow">
      follow us
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@use "../assets/styles/partials/variables" as *;
@use "../assets/styles/partials/mixins" as *;


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

  .follow{
    font-size: 20px;
    text-transform: uppercase;
    font-weight: 600;

    color: $blue;
    display: inline-block;

    padding-top: 4rem;
  }
}
</style>
