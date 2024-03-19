<template>
  <logo />
  <header-popup />
  <div class="popup">
    <headNew />
    <content-popup />
    <next-news />
  </div>
</template>

<script>
import ContentPopup from "~/components/contentPopup.vue";
import HeaderPopup from '~/components/headerPopup.vue';
import logo from "~/components/logo.vue";
import NextNews from "~/components/nextNews.vue";

export default {
  components: { logo, HeaderPopup, ContentPopup, NextNews },
};

</script>

<style lang="scss" scoped>
.popup {

  width: 1536px;
  margin: 0 auto;
  height: 110%;
  overflow: auto;

  background-color: #fff;
}

@media (width: 375px) {
  .popup {
    width: 352px;
    top: 0;
    overflow-y: hidden;
    background-color: #fff;
  }
}
</style>