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
        <div class="row h-100 align-items-center">
          <!-- Logo -->
          <div class="col-4">
            <img
              src="../assets/images/avada-movers-logo.png"
              alt="avada-movers-logo"
            />
          </div>

          <!-- Navbar -->
          <div class="col-8">
            <nav class="navbar d-flex justify-content-end">
              <div>
                <a
                  class="navbar-brand nav-links mx-4"
                  href="#"
                  v-for="(item, id) in navbarArray"
                  :key="id"
                >
                  {{ item.link }}</a
                >
                <button type="button" class="btn btn-denim ms-4">
                  FREE QUOTE
                </button>
              </div>
            </nav>
          </div>
        </div>
      </div>
    </section>
  </header>
</template>

<script>
export default {
  name: "Header",
  props: ["navbarArray"],
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/_variables.scss";
header {
  width: 100%;
  height: 160px;
  position: fixed;
  top: 0;
  left: 0;
  #top-header {
    height: 50px;
    background-color: $lima-dark-vibrant;
    color: white;
    span {
      font-size: 1em;
    }
  }

  #bottom-header {
    height: 110px;
    .nav-links {
      color: $shark-dark-muted;
      font-size: 1em;
      font-weight: 700;
    }
    .nav-links:hover {
      color: $lima-dark-vibrant;
    }

    .btn-denim {
      background-color: $denim-vibrant;
      border-radius: 30px;
      padding: 10px 40px;
      color: white;
      font-size: 0.9em;
      font-weight: 700;
    }
  }
}
</style>