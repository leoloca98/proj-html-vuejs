<template>
  <footer>
    <div class="footer-menu d-flex justify-content-center align-items-center">
      <div class="general-container">
        <div class="block"></div>
      </div>
    </div>
    <div class="copyright"></div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped lang="scss">
footer {
  height: 60vh;
  width: 100%;

  .footer-menu {
    height: 88%;
    width: 100%;
    background-color: darkblue;

    .block {
      height: 350px;
      width: 1100px;
      background-color: limegreen;
    }
  }

  .copyright {
    height: 12%;
    width: 100%;
    background-color: black;
  }
}
</style>