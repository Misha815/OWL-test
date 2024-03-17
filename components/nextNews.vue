<template>
  <div class="h2">
    <span>Следующая статья</span>
  </div>
  <div class="next">
    <div class="rectangle">
      <div class="rectangle__inner">
        <div class="left-item">
          <img src="~/assets/img.png" alt="" />
          <div class="data"><span>06.10.2023</span></div>
        </div>
        <div class="center-item">
          <div class="h3">
            <span
              >Правительство продлило «Льготную ипотеку» и расширило
              «Семейную».</span
            >
          </div>
          <div class="subject">
            <div class="subject__inner">
              <div class="media">
                <span>в СМИ</span>
              </div>
              <div class="sale">
                <span>Акция</span>
              </div>
            </div>
          </div>
        </div>
        <div class="right-item">
          <div class="btn-next"><a href="#"></a></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.h2 {
  width: 1056px;
  margin: 0 auto;
  margin-bottom: 32px;
  span {
    color: #423f3f;
    font-size: 40px;
    margin-top: 16px;
  }
}
.rectangle {
  margin: 0 auto;
  background: no-repeat url("~/assets/mask-news.png");
  height: 228px;
  width: 1056px;

  .rectangle__inner {
    display: flex;
    justify-content: space-between;
    .left-item {
      position: relative;
      .data {
        position: absolute;
        top: 16px;
        left: 16px;
        background-color: #5b4481d9;
        border-radius: 20px;
        width: 110px;
        height: 30px;
        display: flex;
        justify-content: center;
        align-items: center;
        span {
          color: #fff;
        }
      }
    }
    .center-item {
      width: 580px;
      height: 220px;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      .h3 {
        height: 154px;
        span {
          font-size: 24px;
          color: #423f3f;
        }
      }
      .subject {
        .subject__inner {
          margin-bottom: 16px;
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
    }
    .right-item {
      .btn-next {
        width: 80px;
        height: 80px;
        border-radius: 24px;
        background-color: #ffffff;
        box-shadow: 0px 0px 12px #3e4a591f;
        display: flex;
        justify-content: center;
        align-items: center;
        a {
          width: 40px;
          height: 40px;
          border-radius: 24px;

          content: url("~/assets/icon-glyphs.svg");
        }
      }
    }
  }
}
@media (width: 375px) {
  .h2 {
    width: 375px;
    margin: 0 auto;
    margin-bottom: 32px;
    span {
      color: #423f3f;
      font-size: 40px;
      margin-top: 16px;
    }
  }
  .next {
    width: 375px;
    margin: 0 auto;
    .rectangle {
      background: no-repeat url("~/assets/Exclude.png");
      height: 294px;
      max-width: 344px;
      .rectangle__inner {
        display: flex;
        justify-content: space-between;
        flex-direction: column;
        .left-item {
          img {
            max-width: 304px;
            max-height: 164px;
          }
          .data {
            position: absolute;
            top: 16px;
            left: 16px;
            background-color: #5b4481d9;
            border-radius: 20px;
            width: 110px;
            height: 30px;
            display: flex;
            justify-content: center;
            align-items: center;
            span {
              color: #fff;
            }
          }
        }
        .center-item {
          width: 228px;
          height: 48px;
          display: flex;
          flex-direction: column;
          justify-content: space-between;
          .h3 {
            height: 154px;
            span {
              font-size: 14px;
              color: #423f3f;
            }
          }
          .subject {
            .subject__inner {
              margin-bottom: 16px;
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
        }
        .right-item {
          display: flex;
          align-items: center;
          justify-content: center;
          justify-content: flex-end;
          position: relative;
          .btn-next {
            width: 48px;
            height: 48px;
            border-radius: 12px;
            background-color: #ffffff;
            box-shadow: 0px 0px 12px #3e4a591f;
            display: flex;

            align-items: center;
            a {
              width: 17.19px;
              height: 17.19px;
              border-radius: 24px;

              content: url("~/assets/Vector.png");
            }
          }
        }
      }
    }
  }
}
</style>