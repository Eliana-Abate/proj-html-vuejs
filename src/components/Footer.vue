<template>
  <footer>
    <!-- UTILITIES MENU -->
    <section id="utilities">
      <div class="container h-100">
        <div class="row h-100 align-items-center">
          <!-- first column -->
          <div class="col-4 p-4">
            <h4 class="fw-700 mb-5">ABOUT</h4>
            <p class="mb-5">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis
              convallis ex ut sem accumsan vehicula. Integer elit arcu,
              hendrerit id sapien ut, facilisis accumsan arcu.
            </p>
            <img
              src="../assets/images/avada-movers-logo.png"
              alt="avada-movers-logo"
            />
          </div>

          <!-- second column -->
          <div class="col-4 p-4">
            <h4 class="fw-700 mb-5">AVADA MOVERS</h4>
            <ul v-for="(item, id) in footerNavbar" :key="id" class="p-0">
              <li>
                <i class="fas fa-angle-right pe-2"></i>
                {{ item.link }}
              </li>
            </ul>
          </div>

          <!-- third column -->
          <div class="col-4 p-4">
            <h4 class="fw-700 mb-5">RECENT POSTS</h4>
            <ul v-for="(item, id) in postsLink" :key="id" class="p-0">
              <li>
                <i class="fas fa-angle-right pe-2"></i>
                {{ item.link }}
              </li>
            </ul>
          </div>
        </div>
      </div>
    </section>

    <!-- COPYRIGTH INFO AND SOCIAL-->
    <section id="legal-info">
      <div class="container h-100">
        <div class="row h-100 text-center align-content-center">
          <div class="mb-4">
            <span>&copy; </span>
            <span
              >Copyright 2012 - 2021 | Avada Theme by ThemeFusion | All Rights
              Reserved | Powered by WordPress</span
            >
          </div>

          <!-- Social icons -->
          <SocialIcons />
        </div>
      </div>
    </section>
  </footer>
</template>

<script>
import SocialIcons from "@/components/SocialIcons.vue";
export default {
  name: "Footer",
  components: {
    SocialIcons,
  },
  data() {
    return {
      footerNavbar: [
        { link: "Home", id: "1" },
        { link: "Rates", id: "2" },
        { link: "Testimonials", id: "3" },
        { link: "Blog", id: "4" },
        { link: "Free Quote", id: "5" },
      ],

      postsLink: [
        { link: "Heading Out To College?", id: "1" },
        { link: "Moving Your Business?", id: "2" },
        { link: "Outstanding Quality", id: "3" },
        { link: "Cost of Moving", id: "4" },
        { link: "Best Moving Tips", id: "5" },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/_variables.scss";

footer {
  border-top: 15px solid $primary-color;
}

//* -- UTILITIES SECTION --
#utilities {
  height: 500px;
  ul {
    li {
      list-style-type: none;
      cursor: pointer;
    }
    li:hover {
      color: $lima;
    }
  }
}

//* -- COPYRIGTH INFO AND SOCIAL--
#legal-info {
  height: 150px;
  background-color: $primary-color;
  color: $white;
}
</style>