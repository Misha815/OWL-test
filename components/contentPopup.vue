<template>
  <div class="content">
    <div class="content__inner">
      <div class="news-dynamic-text">
        <span>
          Аналитики одного из ведущих игроков на российском рынке кредитования
          объясняют это завершением околонулевых программ и изменением условий
          по ряду
          <span class="link">
            <a href="https://www.vtb.ru/personal/ipoteka/lgotnaya-ipoteka/"
              >программ с господдержкой</a
            ><img src="assets\images\external-link-alt.svg" alt=""
          /></span>
          . При этом специалисты ВТБ прогнозируют в дальнейшем замедление роста
          средней ставки.
        </span>
      </div>

      <div class="content-image">
        <img src="assets\images\content.png" alt="content" />
      </div>
      <div class="news-dynamic-text">
        <span>
          Если во втором полугодии прошлого года средняя ставка по ипотеке
          выросла до 7,38%, к концу года упала до 6,65%, то с начала года она
          выросла: на 1,2 п.п. &mdash; в январе, на 0,19 п.п. &mdash; в феврале
          и, по прогнозам ВТБ, на 0,26 п.п. &mdash; в марте.
        </span>
      </div>
      <div class="news-dynamic-text">
        <span
          >К концу первого квартала средняя ставка по ипотеке достигла 8,3%.
        </span>
      </div>
      <div class="news-dynamic-text">
        <span>
          Самая низкая ставка сейчас действует на рынке новостроек, благодаря
          программам господдержки. По оценке специалистов ВТБ, ее мартовское
          значение составило 5,5%&mdash;5,7%.
        </span>
      </div>
      <div class="news-dynamic-text">
        <span>
          Растущая популярность &laquo;Семейной ипотеки&raquo; в результате ее
          распространения на все семьи с двумя несовершеннолетними детьми и
          адаптация участников рынка к новым условиям &laquo;ипотеки от
          застройщика&raquo; помогут сбалансировать рынок первичной
          недвижимости.
        </span>
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

    .news-dynamic-text {
      color: rgba(113, 112, 112, 1);
      width: 600px;
      margin-bottom: 32px;

      .link {
        a {
          color: rgba(202, 34, 80, 1);
          text-decoration: none;
          &::after {
          }
        }
      }
      br {
        margin-bottom: 50px;
      }
    }
  }
}
@media (width: 375px) {
  .content {
    .content__inner {
      width: 375px;
      margin: 0 auto;
      .content-image {
        display: flex;
        justify-content: center;

        img {
          max-width: 320px;
          max-height: 224px;
        }
      }
      .news-dynamic-text {
        color: rgba(113, 112, 112, 1);
        width: 375px;
        margin-bottom: 32px;

        .link {
          a {
            color: rgba(202, 34, 80, 1);
            text-decoration: none;
            &::after {
            }
          }
        }
      }
    }
  }
}
</style>