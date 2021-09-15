<template>
  <header>
    <!-- TOP HEADER -->
    <section id="top-header">
      <div class="container h-100">
        <div class="row h-100 align-items-center">
          <!-- Contact -->
          <div class="col-6">
            <p class="m-0">Call us for a Free Quote: 1.800.555.6789</p>
          </div>

          <!-- Social Icons -->
          <div class="col-6 text-end">
            <span class="mx-3"><i class="fab fa-facebook-f"></i></span>
            <span class="mx-3"><i class="fab fa-twitter"></i></span>
            <span class="mx-3"><i class="fab fa-instagram"></i></span>
            <span class="ms-3"><i class="fab fa-youtube"></i></span>
          </div>
        </div>
      </div>
    </section>

    <!-- BOTTOM HEADER -->
    <section id="bottom-header">
      <div class="container h-100">
        <div class="row h-100 align-items-center"></div>
      </div>
    </section>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/_variables.scss";
header {
  height: 160px;
  #top-header {
    height: 50px;
    background-color: $lima-dark-vibrant;
    color: white;
    span {
      font-size: 1.1em;
    }
  }

  #bottom-header {
    height: 110px;
    background-color: violet;
  }
}
</style>