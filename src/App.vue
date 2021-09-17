<template>
  <div id="app">
    <Header :navbarArray="headerNavbar" />
    <Main :servicesArray="services" :testimonialsArray="testimonials" />
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
          image: "avada-movers-serviceonephoto-final-400x255",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.",
        },

        {
          title: "We Do All The Lifting",
          id: "2",
          image: "avada-movers-servicetwophoto-final-400x255",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.",
        },

        {
          title: "Coast To Coast",
          id: "3",
          image: "avada-movers-servicethreephoto-final-400x255",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam ac consectetur augue. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.",
        },
      ],

      testimonials: [
        {
          name: "Jonh Doe",
          id: "1",
          comment:
            "“Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent lectus dolor, aliquet sed maximus et, vestibulum pulvinar leo. Vivamus varius pretium fermentum.”",
        },
        {
          name: "Jane Doe",
          id: "2",
          comment:
            "“Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent lectus dolor, aliquet sed maximus et, vestibulum pulvinar leo. Vivamus varius pretium fermentum.”",
        },
        {
          name: "John Smith",
          id: "3",
          comment:
            "“Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent lectus dolor, aliquet sed maximus et, vestibulum pulvinar leo. Vivamus varius pretium fermentum.”",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "./assets/scss/style.scss";
</style>
