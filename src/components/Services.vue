<template>
  <section
    id="services"
    class="d-flex justify-content-center align-items-center"
  >
    <div class="general-container">
      <div class="row flex-column">
        <div class="col business-area"></div>
        <div class="col card-list">
          <div class="row flex-wrap">
            <div class="col-4 card"></div>
            <div class="col-4 card"></div>
            <div class="col-4 card"></div>
            <div class="col-4 card"></div>
            <div class="col-4 card"></div>
            <div class="col-4 card"></div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Services",
};
</script>

<style scoped lang="scss">
@import "../assets/scss/Style.scss";

#services {
  height: 100vh;
  width: 100%;
  background-color: $ServicesFooterBg;

  .row {
    width: 1100px;
    height: 100%;
    border: 2px dashed red;

    .business-area {
      min-height: 180px;
      width: 100%;
      background-color: lightblue;
    }

    .card-list {
      min-height: 520px;
      width: 100%;
      background-color: lightcoral;

      .card {
        height: calc((520px / 2) - 30px);
        width: calc((100% / 3) - 30px);
        margin: 15px;
      }
    }
  }
}
</style>