<template>
  <section class="row">
    <div class="col-4 w-410" v-for="(item, id) in servicesList" :key="id">
      <div class="card-template">
        <div class="img-box">
          <img :src="getImage(item.image)" :alt="item.title" />
        </div>

        <div class="card-template-body text-center">
          <h3 class="fw-700">{{ item.title }}</h3>
          <p>{{ item.description }}</p>
          <div>
            <button type="button" class="btn btn-denim mt-4">READ MORE</button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Card",
  props: ["servicesList"],
  methods: {
    getImage(image) {
      return require(`@/assets/images/${image}.jpg`);
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/_variables.scss";
.card-template {
  border: 20px solid $mercury;
}

.img-box {
  height: 230px;
  border-bottom: 20px solid $mercury;
  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
}
.w-410 {
  width: 410px;
}

.card-template-body {
  padding: 40px 12px;
  h3 {
    color: $denim-vibrant;
  }
  p {
    color: $dove-gray;
  }
}

.col-4:nth-child(2) {
  margin: 0 auto;
}
</style>