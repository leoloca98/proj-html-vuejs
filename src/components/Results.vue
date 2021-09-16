<template>
  <section id="results">
    <div class="row flex-column">
      <div class="col-8 chess"></div>
      <div class="col-4 logos"></div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Results",
};
</script>

<style scoped lang="scss">
@import "../assets/scss/style.scss";

#results {
  height: 90vh;
  width: 100%;
  border: 1px solid black;

  .row {
    height: 100%;
    width: 100%;

    .chess {
      height: 70%;
      width: 100%;
      background-image: url("../assets/img/bg-7.jpg");
      background-position: center;
      background-size: cover;
    }

    .logos {
      height: 30%;
      width: 100%;
      background-color: black;
    }
  }
}
</style>