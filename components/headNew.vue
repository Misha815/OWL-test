<template>
  <div class="header">
    <div class="header__inner">
      <div class="breadcrumb-navigation">
        <ul class="breadcrumb-navigation__inner">
          <li><span class="new">ГЛАВНАЯ</span></li>
          <li><span>НОВОСТИ</span></li>
          <li>
            <span>Средняя ставка по ипотеке в России превысила 8%</span>
          </li>
        </ul>
      </div>
      <div class="subject">
        <div class="subject__inner">
          <div class="media">
            <span>в СМИ</span>
          </div>
          <div class="sale">
            <img src="assets\images\icon-glyphs (1).svg" alt="" /><span
              >Акция</span
            >
          </div>
        </div>
      </div>
      <div class="h1">
        <div class="h1__inner">
          <span>Средняя ставка по ипотеке в России превысила 8%</span>
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
export default {};
</script>

<style lang="scss" scoped>
.header {
  width: 1056px;
  margin: 0 auto;
  .header__inner {
    margin: 0 auto;
    .breadcrumb-navigation {
      .breadcrumb-navigation__inner {
        all: unset;
        display: flex;

        list-style-position: inside;
        li {
          list-style-type: none;
          margin-left: 8px;
          font-size: 16px;

          &::after {
            content: " •";
          }
          &:last-of-type::after {
            content: none;
            margin-left: 0px;
          }
        }
      }
    }
    .subject {
      .subject__inner {
        display: flex;

        .media {
          margin-right: 8px;
          border-radius: 20px;
          text-align: center;
          width: 69px;
          height: 26px;
          border: 1px solid rgba(91, 68, 129, 1);

          span {
            color: rgba(91, 68, 129, 1);
          }
        }
        .sale {
          border: 1px solid rgba(202, 34, 80, 1);
          text-align: center;
          border-radius: 20px;
          width: 88px;
          height: 26px;
          display: flex;
          flex-direction: row;
          justify-content: center;

          img {
          }
          span {
            color: rgba(202, 34, 80, 1);
            &::before {
            }
          }
        }
      }
    }
    .h1 {
      .h1__inner {
        span {
          font-size: 48px;
          color: rgba(66, 63, 63, 1);
          max-width: 1056px;
          display: flex;
        }
      }
    }
    .data-post {
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
    .header__inner {
      .breadcrumb-navigation {
        .breadcrumb-navigation__inner {
          all: unset;
          display: flex;

          width: 375px;

          list-style-position: inside;

          li {
            list-style-type: none;
            margin-left: 8px;
            font-size: 12px;
            overflow: hidden;
            .new {
              display: none;
            }
            &::after {
              content: " •";
            }
            &:first-of-type::after {
              content: none;
              margin-left: 0px;
            }
          }
        }
      }
      .subject {
        .subject__inner {
          display: flex;

          .media {
            margin-right: 8px;
            border-radius: 20px;
            text-align: center;
            width: 69px;
            height: 26px;
            border: 1px solid rgba(91, 68, 129, 1);

            span {
              color: rgba(91, 68, 129, 1);
            }
          }
          .sale {
            border: 1px solid rgba(202, 34, 80, 1);
            text-align: center;
            border-radius: 20px;
            width: 88px;
            height: 26px;
            display: flex;
            flex-direction: row;
            justify-content: center;

            img {
            }
            span {
              color: rgba(202, 34, 80, 1);
              &::before {
              }
            }
          }
        }
      }
      .h1 {
        .h1__inner {
          span {
            font-size: 24px;
            color: rgba(66, 63, 63, 1);
            max-width: 375px;

            display: flex;
          }
        }
      }
      .data-post {
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
}
</style>
