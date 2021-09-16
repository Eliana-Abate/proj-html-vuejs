<template>
  <section class="row">
    <div
      class="col-3 card-template"
      v-for="(item, id) in servicesList"
      :key="id"
    >
      <img src="" alt="" />
      <div class="card-template-body">
        <h4>{{ item.title }}</h4>
        <p>{{ item.description }}</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Card",
  props: ["servicesList"],
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/_variables.scss";
.card-template {
  height: 300px;
  border: 20px solid $mercury;
}

.card-template:nth-child(2) {
  margin: 0px auto;
}
</style>