<template>
  <section
    id="projects"
    class="d-flex justify-content-center align-items-center"
  >
    <div class="general-container">
      <div class="row block flex-column">
        <div class="col-4 projects-menu"></div>
        <div class="col-8 card-list">
          <div class="row flex-wrap justify-content-around">
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
  name: "Projects",
};
</script>

<style scoped lang="scss">
@import "../assets/scss/style.scss";

#projects {
  height: 120vh;
  width: 100%;

  .block {
    min-height: 800px;
    width: 1100px;
    border: 1px dashed red;

    .projects-menu {
      height: 200px;
      width: 100%;
      background-color: slateblue;
    }

    .card-list {
      height: 600px;
      width: 100%;
      background-color: rosybrown;

      .card {
        height: calc((600px / 2) - 30px);
        width: calc((100% / 3) - 30px);
        margin: 15px;
        border-radius: 5%;
      }
    }
  }
}
</style>