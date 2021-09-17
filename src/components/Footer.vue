<template>
  <footer>
    <section id="utilities">
      <div class="container h-100">
        <div class="row h-100 align-items-center">
          <div class="col-4">
            <div></div>
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

          <div class="col-4">
            <h4 class="fw-700 mb-5">AVADA MOVERS</h4>
            <ul v-for="(item, id) in footerNavbar" :key="id" class="p-0">
              <li>
                <i class="fas fa-angle-right pe-2"></i>
                {{ item.link }}
              </li>
            </ul>
          </div>

          <div class="col-4">
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

    <section id="legal-info"></section>
  </footer>
</template>

<script>
export default {
  name: "Footer",
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
  border-top: 15px solid $lima;
}

#utilities {
  height: 450px;
  ul {
    li {
      list-style-type: none;
    }
    li:hover {
      color: $lima;
    }
  }
}

#legal-info {
  height: 150px;
  background-color: $lima;
}
</style>