<template>
  <main>
    <section id="slogan-jumbo" class="jumbotron"></section>
  </main>
</template>

<script>
export default {
  name: "Main",
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/_variables.scss";

#slogan-jumbo {
  height: 800px;
  background-image: url("../assets/images/avada-movers-homeherobackground-final.jpg");
  background-size: 155%;
  background-position-x: center;
  background-position-y: 60px;
  background-repeat: no-repeat;
}
</style>