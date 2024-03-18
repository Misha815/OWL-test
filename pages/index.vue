<template>
  <logo />
  <div class="popup">
    <div class="exit-btn">
      <div class="exit-btn__inner"><button><img src="~/assets/close-icon.svg" alt=""></button></div>
    </div>

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
  position: relative;
  overflow: hidden;

  .exit-btn {
    position: absolute;
    right: 0;

    width: 128px;
    height: 80px;
    background-color: #fff;
    background-image: url('~/assets/close-btn.png');
    box-shadow: 1px 1px 5px 10px #ffffffd6;
    transition: 0.3s ease-in;

    &:hover {
      background-color: #fff;
      transition: 0.3s ease-in;
      opacity: 0.5;
    }

    .exit-btn__inner {
      position: absolute;
      right: 16px;
      top: 12px;



      button {
        all: unset;
        padding: 12px;



        img {

          width: 32px;
          height: 32px;
        }
      }

    }
  }

  border-radius: 16px 16px 0 0;
  background-color: #fff;
}

@media (width: 375px) {
  .popup {
    width: 352px;
    margin: 0 auto;
    position: relative;
    overflow: hidden;



    .exit-btn {
      position: absolute;
      right: 0;

      width: 77px;
      height: 48px;
      background-color: #fff;
      background-image: url('~/assets/close-btn-mobile.png');
      box-shadow: 1px 1px 5px 10px #ffffffd6;

      .exit-btn__inner {
        position: absolute;
        right: 7.9px;
        top: 7.2px;

        button {
          all: unset;
          padding: 7.2px;

          img {

            width: 19px;
            height: 19px;
          }


        }

      }
    }

    border-radius: 16px 16px 0 0;
    background-color: #fff;
  }
}
</style>