<template>
  <main>
    <section id="slogan-jumbo" class="jumbotron">
      <div class="d-flex h-100 justify-content-center align-items-center">
        <div>
          <h6 class="fw-900">MOVING WITHOUT THE HASSLE</h6>
          <h1 class="fw-900 my-4">WE MAKE IT SIMPLE</h1>
          <h6 class="fw-900">
            PROFESSIONAL SERVICE WITH QUALITY AND CUSTOMER SATISFACTION
          </h6>
        </div>
      </div>
    </section>

    <div
      class="
        spacer
        d-flex
        justify-content-center
        align-items-center
        text-center
      "
    >
      <span
        ><i class="far fa-paper-plane me-3"></i>GET A FREE QUOTE ONLINE
        NOW!</span
      >
    </div>

    <section id="award-jumbo" class="jumbotron">
      <div class="d-flex h-100 align-items-center justify-content-center">
        <div
          class="
            cube
            d-flex
            flex-column
            h-100
            align-items-center
            justify-content-center
          "
        >
          <h6 class="fw-900">HEADACHE FREE</h6>
          <div class="wrap-cube">
            <h2 class="fw-900 my-4">Award Winning Moving Company</h2>
          </div>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac
            augue. Orci varius natoque penatibus et magnis dis parturient
            montes, ridiculus mus. Aliquam enim leo, condimentum facilisis nulla
            sed, cursus arcu. Aliquam enim leo.
          </p>

          <button type="button" class="btn btn-denim mt-4">
            READ OUR TESTIMONIALS
          </button>
        </div>
      </div>
    </section>

    <section id="service-solutions">
      <div class="container py-5">
        <div class="row">
          <div class="text-center">
            <h6 class="fw-900">WE ARE A PROFESSIONAL</h6>
            <h2 class="fw-900 my-4">Full-Service Solution</h2>
          </div>
        </div>

        <div class="row">
          <Card />
        </div>
      </div>
    </section>
  </main>
</template>

<script>
import Card from "@/components/Card.vue";
export default {
  name: "Main",
  components: {
    Card,
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/_variables.scss";

#slogan-jumbo {
  height: 800px;
  padding-top: 60px;
  background-image: url("../assets/images/avada-movers-homeherobackground-final.jpg");
  background-size: 120%;
  background-position-x: center;
  background-position-y: 60px;
  background-repeat: no-repeat;
  h6 {
    color: $dove-gray;
  }
  h1 {
    color: $shark;
    font-size: 4em;
  }
}

.spacer {
  height: 150px;
  background-color: $denim-vibrant;
  color: $white;
  font-size: 1.2em;
  span:hover {
    text-decoration: underline;
  }
}

#award-jumbo {
  height: 600px;
  background: linear-gradient($white, $mercury);
  h6 {
    color: $silver-chalice;
  }
  h2 {
    color: $lima;
    font-size: 3em;
  }
  p {
    color: $shark;
  }
}

#service-solutions {
  height: 100vh;
  background-color: $white;
  h6 {
    color: $silver-chalice;
  }
  h2 {
    color: $lima;
    font-size: 3em;
  }
}
</style>