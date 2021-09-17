<template>
  <div class="social-icons">
    <span class="mx-3"><i class="fab fa-facebook-f"></i></span>
    <span class="mx-3"><i class="fab fa-twitter"></i></span>
    <span class="mx-3"><i class="fab fa-instagram"></i></span>
    <span class="ms-3"><i class="fab fa-youtube"></i></span>
  </div>
</template>

<script>
export default {
  name: "SocialIcons",
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/_variables.scss";

.fab,
.fas {
  color: $white;
  font-size: 20px;
  cursor: pointer;
}
</style>