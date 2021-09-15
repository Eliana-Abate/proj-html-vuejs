<template>
  <header>
    <section id="top-header">
      <div class="container">
        <div class="row">
          <p>Call us for a Free Quote: 1.800.555.6789</p>
          <p></p>
        </div>
      </div>
    </section>
    <section id="bottom-header"></section>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/_variables.scss";
header {
  height: 160px;
  #top-header {
    height: 50px;
    background-color: $lima-dark-vibrant;
    color: white;
  }
  #bottom-header {
    height: 110px;
    background-color: violet;
  }
}
</style>