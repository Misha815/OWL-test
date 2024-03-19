<template>
  <div class="content">
    <div class="content__inner">
      <div class="news-dynamic-text">
        <span>
          Аналитики одного из ведущих игроков на российском рынке кредитования
          объясняют это завершением околонулевых программ и изменением условий
          по ряду
          <span class="link">
            <a href="https://www.vtb.ru/personal/ipoteka/lgotnaya-ipoteka/">программ с господдержкой</a></span>
          . При этом специалисты ВТБ прогнозируют в дальнейшем замедление роста
          средней ставки.
        </span>
      </div>

      <div class="content-image">
        <img src="assets\content.png" alt="content" />
      </div>
      <div class="news-dynamic-text">
        <p>
          Если во втором полугодии прошлого года средняя ставка по ипотеке
          выросла до 7,38%, к концу года упала до 6,65%, то с начала года она
          выросла: на 1,2 п.п. &mdash; в январе, на 0,19 п.п. &mdash; в феврале
          и, по прогнозам ВТБ, на 0,26 п.п. &mdash; в марте.
        </p> <br>


        <p>К концу первого квартала средняя ставка по ипотеке достигла 8,3%.
        </p> <br>


        <p>
          Самая низкая ставка сейчас действует на рынке новостроек, благодаря
          программам господдержки. По оценке специалистов ВТБ, ее мартовское
          значение составило 5,5%&mdash;5,7%.
        </p> <br>


        <p>
          Растущая популярность &laquo;Семейной ипотеки&raquo; в результате ее
          распространения на все семьи с двумя несовершеннолетними детьми и
          адаптация участников рынка к новым условиям &laquo;ипотеки от
          застройщика&raquo; помогут сбалансировать рынок первичной
          недвижимости.
        </p> <br>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.content {
  .content__inner {

    width: 1056px;
    margin: 0 auto;

    .content-image {
      margin-bottom: 32px;

      img {
        width: 1056px;
        height: 600px;
      }
    }

    .news-dynamic-text {
      color: rgba(113, 112, 112, 1);
      max-width: 600px;
      margin-bottom: 32px;

      span {
        width: 600px;
        height: 180px;
        font-size: 16px;
        margin-bottom: 32px;

        .link {

          a {
            color: rgba(202, 34, 80, 1);
            text-decoration: none;

            &::after {
              content: ' ' url("~/assets/external-link-alt.svg");
            }
          }
        }
      }
    }

  }
}

@media (width: 375px) {
  .content {
    .content__inner {
      width: 1056px;
      margin: 0 auto;

      .content-image {
        margin-bottom: 32px;
        margin-left: 16px;

        img {
          width: 320px;
          height: 224px;
        }
      }

      .news-dynamic-text {
        color: rgba(113, 112, 112, 1);
        max-width: 312px;
        margin-bottom: 32px;
        margin-left: 16px;

        span {
          width: 312px;
          min-height: 528px;
          font-size: 16px;
          padding-bottom: 16px;
          line-height: 12px;


          .link {
            a {
              color: rgba(202, 34, 80, 1);
              text-decoration: none;

              &::after {
                content: ' ' url("~/assets/external-link-alt.svg");
              }
            }
          }
        }
      }

    }
  }
}
</style>