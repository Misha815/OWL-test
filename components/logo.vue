<template>
  <div class="logo"></div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.logo {
  background-image: url("~/assets/body-menu.png");
  margin: 0 auto;
  width: 1586px;
  height: 100px;
}
@media (max-width: 400px) {
  .logo {
    background-image: none;
    background-image: url("~/assets/mob-top-menu.png");
    margin: 0 auto;
    width: 360px;
    height: 54px;
  }
}
</style>