
<template>
  <logo />
  <div class="popup">
    <headNew />
    <content-popup />
    <next-news />
  </div>
</template>

<script>
import ContentPopup from "~/components/contentPopup.vue";
import logo from "~/components/logo.vue";
import NextNews from "~/components/nextNews.vue";
export default {
  components: { logo, ContentPopup, NextNews },
};
</script>


<style lang="scss" scoped>
.popup {
  width: 1536px;
  margin: 0 auto;
}
@media (width: 375px) {
  .popup {
    width: 375px;
  }
}
</style>
