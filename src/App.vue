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
      services: [
        {
          title: "Two Man Teams",
          id: "1",
          image: "#",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.",
        },

        {
          title: "We Do All The Lifting",
          id: "2",
          image: "#",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.",
        },

        {
          title: "Coast To Coast",
          id: "3",
          image: "#",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "./assets/scss/style.scss";
</style>
