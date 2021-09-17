<template>
  <footer>
    <div class="footer-menu">
      <div
        class="
          general-container
          d-flex
          justify-content-center
          align-items-center
        "
      >
        <div class="block text-white">
          <div class="row h-100">
            <div class="col-3 h-100">
              <img
                class="img-logo"
                src="../assets/img/logo.png"
                alt="Logo NexGen"
              />
              <p class="mt-3 mb-4">
                A Functional HTML Template for Corporate & Business
              </p>
              <div class="mb-2">
                <i class="fas fa-phone-alt"></i>
                +1 (305) 1234-5678
              </div>
              <div class="mb-2">
                <i class="fas fa-envelope"></i>
                hello@example.com
              </div>
              <div class="mb-5">
                <i class="fas fa-map-marker-alt"></i>
                Main Avenue, 987
              </div>
              <span class="button-empty text-white">GET IN TOUCH</span>
            </div>
            <div class="col-9 h-100">
              <div class="row h-100">
                <div
                  v-for="(link, index) in footerLinks"
                  :key="index + '*'"
                  class="col-4 p-4"
                >
                  <h4 class="mb-5">{{ link.name }}</h4>
                  <ul class="list-item">
                    <li
                      v-for="(item, index) in link.list"
                      :key="index + '#'"
                      class="text-secondary"
                    >
                      <i class="fas fa-greater-than me-2"></i>{{ item.list }}
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="copyright text-secondary">
      <div
        class="
          general-container
          d-flex
          justify-content-between
          align-items-center
        "
      >
        <div>Enjoy the low price. We are tracking any intention of piracy.</div>
        <div>
          <i class="far fa-copyright"></i> 2020 NEXGEN is Proudly Powered by
          <span class="principal-color">Codings</span>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      footerLinks: [
        {
          name: "About",
          list: [
            {
              list: "The Company",
            },
            {
              list: "Istitunional",
            },
            {
              list: "Social & Events",
            },
            {
              list: "Innovation",
            },
            {
              list: "Environment",
            },
            {
              list: "Technology",
            },
          ],
        },
        {
          name: "Services",
          list: [
            {
              list: "Audit & Assurance",
            },
            {
              list: "Financial Advisory",
            },
            {
              list: "Analytics M&A",
            },
            {
              list: "Middle Marketing",
            },
            {
              list: "Legal Consulting",
            },
            {
              list: "Reguilatory Risk",
            },
          ],
        },
        {
          name: "Support",
          list: [
            {
              list: "Responsibility",
            },
            {
              list: "Term of Use",
            },
            {
              list: "About Cookies",
            },
            {
              list: "Privacy Policy",
            },
            {
              list: "Accessibility",
            },
            {
              list: "Information",
            },
          ],
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets//scss/style.scss";
footer {
  height: 60vh;
  width: 100%;

  .footer-menu {
    height: 88%;
    width: 100%;
    background-color: $CompanyBg;

    .block {
      height: 300px;
      width: 1050px;

      .list-item {
        display: inline-block;
      }
    }
  }

  .copyright {
    height: 12%;
    width: 100%;
    background-color: black;
  }
}
</style>