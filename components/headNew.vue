<template>
  <div class="header">
    <div class="header__inner">

      <div class="breadcrumb-navigation">
        <ul class="breadcrumb-navigation__inner">
          <li><span class="new">главная</span></li>
          <li><span>новости</span></li>
          <li>
            <span>Средняя ставка по ипотеке в России превысила 8%</span>
          </li>
        </ul>
      </div>
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


    padding-top: 84px;



    .breadcrumb-navigation {
      margin-bottom: 32px;

      .breadcrumb-navigation__inner {
        all: unset;
        display: flex;

        list-style-position: inside;

        li {


          list-style-type: none;
          margin-left: 8px;

          span {
            margin: 0 auto;
            font-size: 16px;
            font-weight: 500;
          }

          letter-spacing: 4%;
          text-transform: uppercase;


          &::after {

            content: " •";
          }

          &:last-of-type::after {
            content: none;
            margin-left: 0px;

          }

          &:last-child {
            color: #423f3f94;
          }
        }
      }
    }

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


      .breadcrumb-navigation {
        width: 352px;
        height: 48px;

        margin: 0 auto;


        .breadcrumb-navigation__inner {



          display: flex;
          white-space: nowrap;
          overflow: hidden;


          li {
            text-transform: uppercase;

            list-style-type: none;
            margin-left: 8px;
            font-size: 12px;
            font-weight: bolder;

            span {
              margin: 0 auto;
              font-size: 12px;
              font-weight: 500;
            }

            letter-spacing: 4%;
            text-transform: uppercase;

            &::after {
              content: " •";
            }

            &:first-child {
              overflow: hidden;
            }

            &:last-of-type::after {
              content: none;
              margin-left: 0px;

            }

            &:last-child {
              color: #423f3f94;
            }
          }
        }
      }

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