<template>
  <div class="col-4">
    <div class="card-template">
      <img src="" alt="" />
      <div class="card-template-body">
        <h4></h4>
        <p></p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/_variables.scss";
.card-template {
  height: 300px;
  border: 20px solid $mercury;
}
</style>