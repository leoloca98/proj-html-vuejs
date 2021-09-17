<template>
  <section id="touch" class="">
    <div
      class="general-container d-flex justify-content-center align-items-center"
    >
      <div class="block">
        <div class="row">
          <div class="col-8 border border-danger"></div>
          <div class="col-4 border border-danger"></div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Touch",
};
</script>

<style scoped lang="scss">
@import "../assets/scss/style.scss";

#touch {
  height: 90vh;
  width: 100%;
  .block {
    height: 600px;
    width: 1100px;
    .row {
      height: 100%;
      width: 100%;
      .col-8 {
        height: 100%;
        background-color: pink;
      }
      .col-4 {
        height: 100%;
        background-color: salmon;
      }
    }
  }
}
</style>