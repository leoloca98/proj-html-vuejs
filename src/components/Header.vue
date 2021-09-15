<template>
  <header>
    <div class="info-menu">
      <div class="general-container"></div>
    </div>
    <div class="jumbotron">
      <div class="general-container">
        <div
          class="
            row
            m-0
            p-0
            flex-column
            justify-content-center
            align-items-center
          "
        >
          <div class="top-bar-menu"></div>
          <div class="square"></div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped lang="scss">
@import "../assets/scss/style.scss";
header {
  height: 90vh;
  width: 100%;

  .info-menu {
    height: 5vh;
    width: 100%;
    background-color: $HeaderBg;
  }

  .jumbotron {
    height: 85vh;
    background-image: url("../assets/img/bg-parallax.png");
    background-position: center;
    background-repeat: no-repeat;

    .top-bar-menu {
      height: 55px;
      width: 100%;
      background-color: forestgreen;
      margin-bottom: 250px;
    }

    .square {
      height: 250px;
      width: 450px;

      background-color: goldenrod;
    }
  }
}
</style>