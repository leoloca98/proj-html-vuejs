<template>
  <section id="services" class="">
    <div
      class="general-container d-flex justify-content-center align-items-center"
    >
      <div class="row row-block flex-column">
        <div class="col business-area mb-5">
          <div class="row row-business">
            <div class="col-10 col-business">
              <div class="principal-color fw-bolder pb-3">
                OUR BUSINESS AREAS
              </div>
              <h2 class="fs-h2 pb-4">
                Excellence in
                <span class="principal-color effect-color">Services</span>
              </h2>
              <p>
                We are leaders in providing consultancy services with a set of
                cutting-edge-technologies and a team of experienced and renowned
                professionals. These are some options that you can hire.
              </p>
            </div>
            <div
              class="
                col-2 col-button
                d-flex
                justify-content-end
                align-items-end
              "
            >
              <span class="button-touch mb-3">SEE ALL</span>
            </div>
          </div>
        </div>
        <div class="col card-list">
          <div class="row flex-wrap justify-content-between">
            <div
              v-for="service in services"
              :key="service.id"
              class="col-4 card"
            >
              <div class="row row-card">
                <div
                  class="
                    col-10 col-text
                    text-center
                    d-flex
                    flex-column
                    justify-content-center
                    align-items-center
                  "
                >
                  <img :src="service.icon" class="mb-3 icon-size" />
                  <div class="fw-bold fs-5 pb-3">{{ service.title }}</div>
                  <div>{{ service.lorem }}</div>
                </div>
                <div class="col-2 col-arrow">
                  <i class="fas fa-arrow-right principal-color"></i>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Services",
  data() {
    return {
      services: [
        {
          icon: require(`../assets/img/svg/svg-1.svg`),
          title: "Audit & Assurance",
          lorem: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          id: 1001,
        },
        {
          icon: require(`../assets/img/svg/svg-2.svg`),
          title: "Financial Advisory",
          lorem: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          id: 1002,
        },
        {
          icon: require(`../assets/img/svg/svg-3.svg`),
          title: "Analytics and M&A",
          lorem: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          id: 1003,
        },
        {
          icon: require(`../assets/img/svg/svg-4.svg`),
          title: "Middle Marketing",
          lorem: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          id: 1004,
        },
        {
          icon: require(`../assets/img/svg/svg-5.svg`),
          title: "Legal Consulting",
          lorem: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          id: 1005,
        },
        {
          icon: require(`../assets/img/svg/svg-6.svg`),
          title: "Regulatory Risk",
          lorem: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
          id: 1006,
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/Style.scss";

#services {
  height: 100vh;
  width: 100%;
  background-color: $ServicesFooterBg;

  .row-block {
    width: 1050px;
    height: 80%;

    .business-area {
      min-height: 180px;
      width: 100%;

      .row-business {
        min-height: 180px;
        width: 100%;

        .col-business {
          min-height: 160px;
        }

        .col-button {
          min-height: 160px;
        }
      }
    }

    .card-list {
      min-height: 520px;
      width: 100%;

      .card {
        height: calc((480px / 2));
        width: calc((95% / 3));
        border: 0;
        border-radius: 10px;
        padding: 20px;
        margin-bottom: 30px;

        .row-card {
          height: 100%;
          width: 100%;

          .col-text img {
            max-width: 50px;
          }
        }
      }
    }
  }
}
</style>