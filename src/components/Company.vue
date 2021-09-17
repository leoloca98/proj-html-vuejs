<template>
  <section
    id="company"
    class="d-flex justify-content-center align-items-center"
  >
    <div class="row row-block p-0 m-0">
      <div
        class="col-6 network d-flex align-items-center justify-content-center"
      >
        <div class="network-info">
          <div class="about-network mb-4">
            <p class="principal-color mb-4">ABOUT THE NETWORK</p>
            <h2 class="fs-h2 mb-4">
              <span class="effect-color">The</span> Company
            </h2>
            <p>
              For 12 years we have been providing audit and warranty, financial
              advice, risk advice, taxes and related services to select clients
            </p>
          </div>
          <div class="row flex-wrap">
            <div
              v-for="(netwok, index) in networks"
              :key="index + network.title"
              class="col-6 card"
            ></div>
          </div>
        </div>
      </div>
      <div class="col-6 about-bg"></div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Company",
  data() {
    return {
      networks: [
        {
          icon: "award",
          title: "Tradition",
          lorem: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
        },
        {
          icon: "lock",
          title: "Security",
          lorem: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
        },
        {
          icon: "edit",
          title: "Certificate",
          lorem: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
        },
        {
          icon: "graduation-cap",
          title: "Expertise",
          lorem: "Lorem ipsum dolor sit amet consectetur adipiscing elit.",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets//scss/style.scss";

#company {
  height: 90vh;
  width: 100%;

  .row-block {
    width: 100%;
    height: 100%;
    border: 1px dashed red;

    .network {
      background-color: $CompanyBg;

      .network-info {
        height: 600px;
        width: 50%;
        margin-left: 320px;
        background-color: sandybrown;
      }
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