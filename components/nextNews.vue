<template>
  <div class="h2">
    <span>Следующая статья</span>
  </div>
  <div class="next">
    <div class="rectangle">
      <div class="rectangle__inner">
        <div class="left-item">

          <div class="data"><span>06.10.2023</span></div>
        </div>
        <div class="center-item">
          <div class="h3">
            <span>Правительство продлило «Льготную ипотеку» и расширило
              «Семейную».</span>
          </div>

          <div class="subject-container">
            <subject />
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
    display: flex;
    font-family: 'Unbounded';
    color: rgba(66, 63, 63, 1);

    font-weight: bolder;
    font-size: 40px;
    margin-top: 16px;
  }
}

.rectangle {
  margin: 0 auto;
  background: no-repeat url("~/assets/mask-news.png");
  width: 1056px;
  padding-bottom: 128px;

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


          display: flex;
          font-family: 'Unbounded';
          color: rgba(66, 63, 63, 1);

          font-weight: bolder;

        }
      }

      .subject-container {
        padding-bottom: 16px;
        display: flex;
        padding-left: 16px;
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
    width: 334px;
    margin: 0 auto;
    margin-bottom: 32px;


    span {
      display: flex;
      font-family: 'Unbounded';
      color: rgba(66, 63, 63, 1);

      font-weight: bolder;
      font-size: 20px;
      margin-top: 16px;
    }
  }

  .rectangle {
    margin: 0 auto;
    background: no-repeat url("~/assets/mask-news.png");
    width: 344px;
    padding-bottom: 128px;

    .rectangle__inner {
      width: 312px;
      height: 294px;
      display: flex;
      flex-direction: column;
      justify-content: center;


      .left-item {
        position: relative;
        background: no-repeat url('~/assets/card-news-mobile.png');
        width: 304px;
        height: 164px;
        z-index: 4;

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
        height: 100px;
        display: flex;
        flex-direction: column;
        justify-content: space-between;

        .h3 {
          width: 288px;
          height: 48px;

          span {
            font-size: 14px;



            font-family: 'Unbounded';
            color: rgba(66, 63, 63, 1);

            font-weight: bolder;

          }
        }

        .subject-container {}

      }

      .right-item {
        .btn-next {
          width: 80px;
          height: 80px;
          border-radius: 24px;
          background-color: #ffffff;
          box-shadow: 0px 0px 12px #3e4a591f;


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
}
</style>