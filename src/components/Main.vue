<template>
  <main>
    <!-- SLOGAN: WE MAKE IT SIMPLE -->
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

    <!-- SPACER BUTTON -->
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

    <!-- Award Winning Moving Company -->
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

    <!-- Full-Service Solutions -->
    <section id="service-solutions">
      <div class="container">
        <div class="row">
          <div class="text-center pb-5">
            <h6 class="fw-900">WE ARE A PROFESSIONAL</h6>
            <h2 class="fw-900 my-4">Full-Service Solution</h2>
          </div>
        </div>

        <Card :servicesList="servicesArray" />
      </div>
    </section>

    <!-- Move With Ease -->
    <section id="move-ease-slogan" class="jumbotron">
      <div class="container h-100">
        <div class="row h-100">
          <div class="ms-auto col-6">
            <div class="d-flex align-items-center h-100">
              <div class="move-banner">
                <div class="d-flex flex-column align-items-center">
                  <h6 class="fw-900">WE REMOVE THE HEADACHE FROM MOVING</h6>
                  <h2 class="fw-900">Move With Ease</h2>
                  <div class="hr-spacer my-2"></div>
                  <p class="pt-4">
                    With our super simple service we can take you from getting a
                    quote, right through to being in your new home with all of
                    your belongings securely packed and safely delivered, even
                    in the rooms of your choice.
                  </p>
                  <div>
                    <button type="button" class="btn btn-denim mt-4">
                      GET A FREE QUOTE NOW
                    </button>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Testimonials -->
    <section id="testimonials">
      <div class="container">
        <div class="row">
          <div class="text-center pb-5">
            <h6 class="fw-900">HAPPY CUSTOMERS</h6>
            <h2 class="fw-900 my-4">Testimonials</h2>
          </div>
        </div>

        <TestimonialCard :testimonialsList="testimonialsArray" />

        <div class="row mt-3">
          <div class="d-flex justify-content-center">
            <button type="button" class="btn btn-denim mt-4">
              READ MORE TESTIMONIALS
            </button>
          </div>
        </div>
      </div>
    </section>

    <!-- Request Free Quote -->
    <section id="request-quote-jumbo" class="jumbotron">
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
          <h2 class="fw-900 my-4">Request A Free Quote</h2>

          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac
            consectetur augue. Orci varius natoque penatibus et magnis dis
            parturient montes, nascetur ridiculus mus.
          </p>

          <button type="button" class="btn btn-denim mt-4">CLICK HERE</button>
        </div>
      </div>
    </section>
  </main>
</template>

<script>
import Card from "@/components/Card.vue";
import TestimonialCard from "@/components/TestimonialCard.vue";

export default {
  name: "Main",
  props: ["servicesArray", "testimonialsArray"],
  components: {
    Card,
    TestimonialCard,
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/_variables.scss";

//* -- SLOGAN: WE MAKE IT SIMPLE --
#slogan-jumbo {
  height: 630px;
  padding-top: 50px;
  background-image: url("../assets/images/avada-movers-homeherobackground-final.jpg");
  background-size: 118%;
  background-position-x: center;
  background-position-y: 50px;
  background-repeat: no-repeat;
  h6 {
    color: $dove-gray;
  }
  h1 {
    color: $shark;
    font-size: 4em;
  }
}

//* -- SPACER BUTTON --
.spacer {
  height: 140px;
  background-color: $denim-vibrant;
  color: $white;
  font-size: 1.2em;
  letter-spacing: 2px;
  cursor: pointer;
}

.spacer:hover {
  filter: brightness(1.15);
  span {
    text-decoration: underline;
  }
}

//* -- AWARD WINNING MOVING COMPANY --
#award-jumbo {
  height: 600px;
  background: linear-gradient($white, $mercury);
}

//* -- FULL-SERVICE SOLUTIONS --
#service-solutions {
  background-color: $white;
  height: 1000px;
}
//! COMMON STYLE: full-service and testimonials sections
#service-solutions,
#testimonials {
  height: 1000px;
  display: flex;
  justify-content: center;
  align-items: center;
}

//* -- MOVE WITH EASE --
#move-ease-slogan {
  height: 700px;
  background-image: url("../assets/images/avada-movers-movewithease-background-new.jpg");
  background-size: cover;
  .move-banner {
    width: 100%;
    height: 420px;
    padding: 50px;
    background-color: $primary-color;
    border: 15px solid $hippie-green;
    color: $white;
    h2,
    h6,
    p {
      color: $white;
    }
  }
}

.hr-spacer {
  width: 75%;
  height: 0.5px;
  background-color: $oslo-gray;
}

//* TESTIMONIALS
#testimonials {
  background-image: url("../assets/images/avada-movers-testimonial-background.jpg");
  background-size: 140%;
  background-position: center;
  background-repeat: no-repeat;
}

//* REQUEST FREE QUOTE
#request-quote-jumbo {
  height: 500px;
  background-image: url("../assets/images/avada-movers-request-quote-background.jpg");
  background-position: center;
  background-size: cover;
}
</style>