<template>
  <footer>
    <section id="utilities">
      <div class="container h-100">
        <div class="row h-100 align-items-center">
          <div class="col-4">
            <h4 class="fw-700">ABOUT</h4>
            <p>
              Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis
              convallis ex ut sem accumsan vehicula. Integer elit arcu,
              hendrerit id sapien ut, facilisis accumsan arcu.
            </p>
            <img
              src="../assets/images/avada-movers-logo.png"
              alt="avada-movers-logo"
            />
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
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/_variables.scss";
footer {
  border-top: 15px solid $lima;
}

#utilities {
  height: 450px;
}

#legal-info {
  height: 150px;
  background-color: $lima;
}
</style>