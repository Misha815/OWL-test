<template>
  <div class="logo-container">
    <div class="logo"></div>
  </div>

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
  .logo-container {
    position: relative;

    width: 375px;
    padding-left: 8px;

    .logo {
      background: no-repeat url("~/assets/mob-top-menu.png");


      height: 62px;
      position: fixed;
      background-color: rgba(128, 120, 120, 0.98);
      top: 0px;
    }
  }
}
</style>