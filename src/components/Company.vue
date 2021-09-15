<template>
  <section
    id="company"
    class="d-flex justify-content-center align-items-center"
  >
    <div class="row p-0 m-0">
      <div class="col-6 network">
        <div class="general-container"></div>
      </div>
      <div class="col-6 about-bg"></div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Company",
};
</script>

<style scoped lang="scss">
@import "../assets//scss/style.scss";

#company {
  height: 90vh;
  width: 100%;

  .row {
    width: 100%;
    height: 100%;
    border: 1px dashed red;

    .network {
      background-color: $CompanyBg;
    }

    .about-bg {
      background-image: url("../assets/img/about-4.jpg");
      background-position: center;
      background-size: cover;
      background-repeat: no-repeat;
    }
  }
}
</style>