<template>
  <div class="header">
    <div class="header__inner">


      <div class="subject-container">
        <subject />
      </div>

      <div class="h1">
        <div class="h1__inner">
          <span>
            <h1>Средняя ставка по ипотеке в России превысила 8%</h1>
          </span>
        </div>
      </div>
      <div class="data-post">
        <div class="data-post__inner">
          <span>06.10.2023</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import subject from './subject.vue';
export default {
  components: { subject },
};
</script>

<style lang="scss" scoped>
.header {

  width: 1056px;
  margin: 0 auto;

  .header__inner {


    .subject-container {


      margin-bottom: 32px;
    }

    .h1 {
      margin-bottom: 16px;

      .h1__inner {
        span {
          h1 {

            font-size: 48px;
            max-width: 1056px;
            display: flex;
            font-family: 'Unbounded';
            color: rgba(66, 63, 63, 1);

            font-weight: bolder;

          }

        }
      }
    }

    .data-post {
      margin-bottom: 32px;

      .data-post__inner {
        span {
          color: rgba(207, 207, 207, 1);
          font-size: 16px;
          text-decoration: underline rgba(207, 207, 207, 1);
          text-underline-offset: 4px;
        }
      }
    }
  }
}

@media (width: 375px) {
  .header {

    max-width: 352px;


    .header__inner {

      padding-top: 18px;




      .subject-container {
        margin-bottom: 16px;
        display: flex;
        margin-left: 16px;
      }

      .h1 {
        margin-left: 16px;
        margin-bottom: 16px;


        .h1__inner {


          span {


            h1 {

              font-size: 24px;
              max-width: 352px;

              letter-spacing: 0%;
              font-family: 'Unbounded';
              color: rgba(66, 63, 63, 1);

              font-weight: bolder;

            }

          }
        }
      }

      .data-post {
        margin-left: 16px;
        margin-bottom: 32px;

        .data-post__inner {
          span {
            color: rgba(207, 207, 207, 1);
            font-size: 14px;
            text-decoration: underline rgba(207, 207, 207, 1);
            text-underline-offset: 4px;
          }
        }
      }
    }
  }
}
</style>