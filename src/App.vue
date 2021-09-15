<template>
  <div id="app">
    <Header :navbarArray="headerNavbar" />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Main from "@/components/Main.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
  data() {
    return {
      headerNavbar: [
        { link: "Home", id: "1" },
        { link: "Rates", id: "2" },
        { link: "Testimonials", id: "3" },
        { link: "FAQ", id: "4" },
        { link: "Blog", id: "5" },
        { link: "Contact", id: "6" },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "./assets/scss/style.scss";
</style>
