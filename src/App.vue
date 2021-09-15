<template>
  <div id="app">
    <Header />
    <Services />
    <Company />
    <Main />
    <Footer />
  </div>
</template>

<script>
/*

1- Header
2- Jumbotron (menu-bar)
3- Services Section (card -> logos svg -> hover effects)
4- Company Section (2 col background + position + dots effect)
5- Projects Section (menu-link + card)
6- Results Section (bgc-img + opacity + row-column)
7- Touch Section (2 col -> form / address)
8- Footer (2 col-> address / footer-link-menu + copyright)

*/
import Header from "@/components/Header.vue";
import Services from "@/components/Services.vue";
import Company from "@/components/Company.vue";
import Main from "@/components/Main.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Services,
    Company,
    Main,
    Footer,
  },
};
</script>

<style lang="scss">
@import "../src/assets/scss/_vars.scss";
</style>
