<template>
  <main>
    <section id="slogan-jumbo" class="jumbotron">
      <div class="row h-100 align-items-center">
        <div>
          <h6 class="fw-900">MOVING WITHOUT THE HASSLE</h6>
          <h1 class="fw-900 my-4">WE MAKE IT SIMPLE</h1>
          <h6 class="fw-900">
            PROFESSIONAL SERVICE WITH QUALITY AND CUSTOMER SATISFACTION
          </h6>
        </div>
      </div>
    </section>

    <div class="spacer row align-items-center text-center">
      <span
        ><i class="far fa-paper-plane me-3"></i>GET A FREE QUOTE ONLINE
        NOW!</span
      >
    </div>
  </main>
</template>

<script>
export default {
  name: "Main",
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
}
</style>