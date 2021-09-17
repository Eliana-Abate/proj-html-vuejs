<template>
  <header>
    <!-- TOP HEADER -->
    <section id="top-header">
      <div class="container h-100">
        <div class="row h-100 align-items-center">
          <!-- Contact -->
          <div class="col-6">
            <p class="m-0">
              <i class="fas fa-phone me-3"></i>Call us for a Free Quote:
              1.800.555.6789
            </p>
          </div>

          <!-- Social Icons -->
          <div class="col-6 text-end">
            <SocialIcons />
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
import SocialIcons from "@/components/SocialIcons.vue";
export default {
  name: "Header",
  components: {
    SocialIcons,
  },
  props: ["navbarArray"],
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/_variables.scss";
header {
  width: 100%;
  height: 160px;
  position: absolute;
  top: 0;
  left: 0;
  #top-header {
    height: 50px;
    background-color: $lima-dark-vibrant;
    color: $white;
    font-size: 0.9em;
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
  }
}
</style>