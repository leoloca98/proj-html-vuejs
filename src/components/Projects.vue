<template>
  <section id="projects" class="">
    <div
      class="general-container d-flex justify-content-center align-items-center"
    >
      <div class="row block flex-column">
        <div class="col-4 projects-menu text-center">
          <div class="principal-color fw-bolder pb-3">
            WE DO MORE FOR EVERYONE
          </div>
          <h2 class="fs-h2 pb-5">
            Actions &
            <span class="principal-color effect-color">Projects</span>
          </h2>
          <ul class="d-flex justify-content-around">
            <li
              v-for="(project, index) in projects"
              :key="index + project.link"
              :class="
                project.link == 'ALL' ? 'effect-color principal-color' : ''
              "
            >
              {{ project.link }}
            </li>
          </ul>
        </div>
        <div class="col-8 card-list">
          <div class="row flex-wrap justify-content-around">
            <div
              v-for="(card, index) in cards"
              :key="index + '-' + index"
              class="col-4 card-projects position-relative"
            >
              <span class="text-white card-title position-absolute">{{
                card.title
              }}</span>
              <img :src="card.img" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Projects",
  data() {
    return {
      projects: [
        {
          link: "ALL",
        },
        {
          link: "INSTITUTIONAL",
        },
        {
          link: "SOCIAL",
        },
        {
          link: "EVENTS",
        },
        {
          link: "INNOVATION",
        },
        {
          link: "ENVIRONMENT",
        },
        {
          link: "TECHNOLOGY",
        },
      ],
      cards: [
        {
          img: require("../assets/img/project-1.jpg"),
          title: "Academic professional program in social media",
        },
        {
          img: require("../assets/img/project-2.jpg"),
          title: "President's speech at the annual meeting",
        },
        {
          img: require("../assets/img/project-3.jpg"),
          title: "International business trip in Shanghai",
        },
        {
          img: require("../assets/img/project-4.jpg"),
          title: "Technology workshop with education theme",
        },
        {
          img: require("../assets/img/project-5.jpg"),
          title: "Donation of clothes and food to the parter NGO",
        },
        {
          img: require("../assets/img/project-6.jpg"),
          title: "Confraternization of the procurement team",
        },
      ],
    };
  },
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

    .projects-menu {
      height: 200px;
      width: 100%;
    }

    .card-list {
      height: 600px;
      width: 100%;

      .card-projects {
        height: calc((600px / 2) - 20px);
        width: calc((100% / 3) - 20px);
        margin: 10px;
        border-radius: 5%;

        .card-title {
          z-index: 1;
          left: 1%;
          bottom: 10%;
          font-weight: 700;
          font-size: 22px;
          text-align: center;
        }

        img {
          height: 100%;
          width: 100%;
          object-fit: cover;
          border-radius: 5%;
          filter: brightness(65%);
        }
      }
    }
  }
}
</style>