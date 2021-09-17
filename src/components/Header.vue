<template>
  <header>
    <div class="info-menu text-white">
      <div class="general-container">
        <div class="row justify-content-between">
          <div class="col-7 hours">
            <span
              ><i class="fas fa-clock"></i> Open Hours: Mon-Sat - 9.00 -
              18.00</span
            >
          </div>
          <div class="col-5 info d-flex justify-content-between">
            <span><i class="fas fa-phone-alt"></i> +1 (305) 1234-5678</span>
            <span><i class="fas fa-envelope"></i> hello@example.com</span>
            <span><i class="fab fa-facebook-f"></i></span>
            <span><i class="fab fa-twitter"></i></span>
            <span><i class="fab fa-linkedin-in"></i></span>
          </div>
        </div>
      </div>
    </div>
    <div class="jumbotron">
      <div class="general-container h-100">
        <div
          class="
            row
            top-bar-menu
            justify-content-between
            align-items-center
            pt-3
          "
        >
          <div class="col-4">
            <img class="img-logo" src="../assets/img/logo.png" alt="Logo" />
          </div>
          <div class="col-8 d-flex justify-content-between align-items-center">
            <li
              v-for="(item, index) in topBarLinks"
              :key="index + '%'"
              :class="item.list == 'GET IN TOUCH' ? 'button-touch' : ''"
            >
              <a href="#" class="link">
                {{ item.list }}
              </a>
            </li>
          </div>
        </div>
        <div class="row something justify-content-center align-items-center">
          <div class="col team text-center">
            <h1 class="pb-4 fs-h1">
              Ready <span class="principal-color effect-color">Team</span>
            </h1>
            <p class="pb-5">
              No matter what your company needs, we will be ready to assist you
              in the best possible way
            </p>
            <span class="me-4 button-touch"
              ><a class="text-white" href="#">GET IN TOUCH</a></span
            >
            <span class="ms-4 button-empty"
              ><a class="principal-color" href="#">READ MORE</a></span
            >
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      topBarLinks: [
        {
          list: "HOME",
        },
        {
          list: "SERVICES",
        },
        {
          list: "ABOUT",
        },
        {
          list: "PROJECTS",
        },
        {
          list: "RESULTS",
        },
        {
          list: "GET IN TOUCH",
        },
      ],
    };
  },
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
    line-height: 5vh;
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
    }

    .something {
      height: calc(85vh - 55px);

      .team {
        height: 250px;
        max-width: 450px;
      }
    }
  }
}
</style>