<template>
  <section id="results" class="text-white">
    <div class="row flex-column">
      <div class="col-8 chess">
        <div
          class="
            general-container
            d-flex
            justify-content-center
            align-items-center
          "
        >
          <div class="text">
            <span class="principal-color fw-bolder">WHAT WE ARE DOING</span>
            <h2 class="fs-h2 my-5">
              <span class="effect-color">Results</span> in Numbers
            </h2>
            <div class="row justify-content-around py-5">
              <div
                v-for="(number, index) in numbers"
                :key="index + number.n"
                class="col card-number"
              >
                <div class="principal-color fs-2 fw-bold">{{ number.n }}</div>
                <div class="fs-5 fw-bolder">{{ number.of }}</div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-4 logos">
        <div class="general-container">
          <ul class="d-flex align-items-center justify-content-between h-100">
            <li v-for="(partner, index) in partners" :key="index + partner.n">
              <img :src="partner.link" />
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Results",
  data() {
    return {
      numbers: [
        {
          n: "128",
          of: "Certifications",
        },
        {
          n: "230",
          of: "Employees",
        },
        {
          n: "517",
          of: "Customers",
        },
        {
          n: "94",
          of: "Countries Served",
        },
      ],
      partners: [
        {
          link: require(`../assets/img/logo-4.png`),
        },
        {
          link: require(`../assets/img/logo-5.png`),
        },
        {
          link: require(`../assets/img/logo-1.png`),
        },
        {
          link: require(`../assets/img/logo-2.png`),
        },
        {
          link: require(`../assets/img/logo-3.png`),
        },
        {
          link: require(`../assets/img/logo-4.png`),
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/style.scss";

#results {
  height: 90vh;
  width: 100%;

  .row {
    height: 100%;
    width: 100%;

    .chess {
      height: 70%;
      width: 100%;
      text-align: center;
      background-image: url("../assets/img/bg-7.jpg");
      background-position: center;
      background-size: cover;

      .text {
        height: 70%;
        width: 1050px;
      }
    }

    .logos {
      height: 30%;
      width: 100%;
      background-color: #000;

      img {
        max-width: 75px;
      }
    }
  }
}
</style>