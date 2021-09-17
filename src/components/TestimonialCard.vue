<template>
  <section class="row">
    <div class="col-4 w-410" v-for="(item, id) in testimonialsList" :key="id">
      <div class="card-template d-flex flex-column align-items-center">
        <img :src="getImage(item.image)" :alt="item.name" />

        <div class="card-template-body text-center">
          <h3 class="fw-700 mb-4">{{ item.name }}</h3>
          <p class="pt-3">
            <em>{{ item.comment }}</em>
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "testimonialCard",
  props: ["testimonialsList"],
  methods: {
    getImage(image) {
      return require(`@/assets/images/${image}.jpg`);
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/_variables.scss";

img {
  width: 40%;
  border-radius: 50%;
}

.card-template-body {
  padding: 40px 8px;
}

.col-4:nth-child(2) {
  margin: 0 auto;
}
</style>