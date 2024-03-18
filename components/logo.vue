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

@media (max-width: 375px) {
  .logo {


    background: no-repeat url("~/assets/mob-top-menu.png");


    max-width: 357px;
    height: 62px;
  }
}
</style>