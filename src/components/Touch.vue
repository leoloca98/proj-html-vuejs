<template>
  <section id="touch" class="">
    <div
      class="general-container d-flex justify-content-center align-items-center"
    >
      <div class="block">
        <div class="row">
          <div class="col-8 form-message pe-5">
            <span class="principal-color fw-bold">SEND A MESSAGE</span>
            <h2 class="fw-bolder my-4">
              Get in
              <span class="principal-color effect-color">Touch</span>
            </h2>
            <p class="mb-5">
              We will respond to your message as soon as possible.
            </p>
            <div class="form-contact d-flex flex-wrap justify-content-between">
              <input
                type="text"
                placeholder="Name"
                aria-label="First name"
                class="form-control input-message"
              />
              <input
                type="text"
                placeholder="Email"
                aria-label="Last name"
                class="form-control input-message"
              />
              <input
                type="text"
                placeholder="Phone"
                aria-label="First name"
                class="form-control input-message"
              />
              <select
                class="form-select input-message"
                aria-label="Default select "
              >
                <option selected>More Info</option>
                <option value="1">One</option>
                <option value="2">Two</option>
                <option value="3">Three</option>
              </select>
              <textarea
                class="form-control input-message w-100 pb-5"
                aria-label="With textarea"
                placeholder="Message"
              ></textarea>
              <span class="button-touch">SEND</span>
            </div>
          </div>
          <div class="col-4 contact-us px-3">
            <h4 class="fw-bold mb-4">Example Inc.</h4>
            <p class="mb-4">
              Lorem ipsum dolor sit amet, consectetur adipiscinding elit.
            </p>
            <p class="mb-4">
              Praesent diam lacus, dapibus sed imperdiet consectetur.
            </p>
            <div class="principal-color mb-3">
              <i class="fas fa-phone-alt circle"></i>
              +1 (305) 1234-5678
            </div>
            <div class="principal-color mb-3">
              <i class="fas fa-envelope circle"></i>
              hello@example.com
            </div>
            <div class="principal-color mb-3">
              <i class="fas fa-map-marker-alt circle"></i>
              Main Avenue, 987
            </div>
            <br />
            <span class="button-empty">VIEW MAP</span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Touch",
};
</script>

<style scoped lang="scss">
@import "../assets/scss/style.scss";

#touch {
  height: 90vh;
  width: 100%;

  .block {
    height: 600px;
    width: 1100px;

    .row {
      height: 100%;
      width: 100%;

      .form-message {
        height: 100%;

        .input-message {
          border: 0;
          padding: 10px 15px;
          width: calc((100% / 2) - 15px);
          display: inline-block;
          background-color: rgba(211, 211, 211, 0.747);
          margin-bottom: 30px;
        }
      }

      .contact-us {
        height: 100%;
      }
    }
  }
}
</style>