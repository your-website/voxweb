<template>
    <div class="cards">
        <div class="cards__item">
            <div class="cards__container">
                <img class="cards__img" src="../../assets/images/img__one.jpg" alt="">
                <a class="cards__link">от 118 112 &#8381;</a>
            </div>
            <h3 class="cards__title-country">ИТАЛИЯ</h3>
            <h2 class="cards__content-title">Под небом Тосканы</h2>
            <p class="cards__paragraph-countries">Сансеполькро — (Перуджа) — Ассизи — Губбио — (Сиена) — Ла Верна — Ангиари — Монтерки — Ареццо — Кортона — (Пиенца) - (Монтепульчано)</p>
            <p class="cards__paragraph-date">8 дней / 7 ночей Русский язык 27.04.19 - 04.05.19 и еще 15 дат</p>
            <a class="cards__link-sall-out">Авиаперелет включен!</a>
        </div>
        <div class="cards__item">
            <div class="cards__container">
                <img class="cards__img" src="../../assets/images/img__two.jpg" alt="">
                <a class="cards__link">140 715 &#8381;</a>
            </div>
            <h3 class="cards__title-country">ИСЛАНДИЯ</h3>
            <h2 class="cards__content-title">Майские каникулы в Исландии</h2>
            <p class="cards__paragraph-countries">Рейкьявик — Тингвеллир — Гюдльфосс — Скафтафедль — Сельяландсфосс — Скоугафосс — Йёкюльсаурлоун — Голубая Лагуна — Снайфельсйёкутль — Arnarstapi — Рейкьявик</p>
            <p class="cards__paragraph-date">8 дней / 7 ночей Русский язык 27.04.19 - 04.05.19</p>
        </div>
        
        <div class="cards__item">
            <div class="cards__container">
                <img class="cards__img" src="../../assets/images/img__three.jpg" alt="">
                <a class="cards__link">37 302 &#8381;</a>
            </div>
            <h3 class="cards__title-country">ТУРЦИЯ</h3>
            <h2 class="cards__content-title">Открытие Турции</h2>
            <p class="cards__paragraph-countries">Стамбул — Анкара — Каппадокия — Конья — Памуккале — Эфес — Кушадасы — Пергам — Ассос — Троя — Стамбул</p>
            <p class="cards__paragraph-date">8 дней / 7 ночей Русский язык 28.04.19 - 05.05.19 и еще 3 даты</p>
        </div>
        <div class="cards__item">
            <div class="cards__container">
                <img class="cards__img" src="../../assets/images/img__four.jpg" alt="">
                <a class="cards__link">145 000 &#8381;</a>
            </div>
            <h3 class="cards__title-country">ИТАЛИЯ</h3>
            <h2 class="cards__content-title">От Свальбарда до Груманта</h2>
            <p class="cards__paragraph-date">8 дней / 7 ночей Русский язык 27.04.19 - 04.05.19 и еще 15 дат</p>
            <a class="cards__link-sall-out">Гарантированный тур!</a>
        </div>
    </div>
</template>

<script>
  export default {
    components: {
    },
    data: function() {
        return {
        };
    },
   
  }
</script>

<style lang="scss">
    .cards {
        display: grid;
        grid-template-columns: 380px 380px;
        grid-gap: 20px;

        @media screen and (max-width: 860px) {
            grid-template-columns: 380px;
        }

        @media screen and (max-width: 430px) {
            grid-template-columns: 300px;
        }
    }

    .cards__item {

    }

    .cards__container {
        position: relative;
        max-width: 380px;
        height: 218px;
        margin-bottom: 10px;

        @media screen and (max-width: 430px) {
            max-width: 300px;
        }
    }

    .cards__img {
        height: 100%;

        @media screen and (max-width: 430px) {
            max-width: 300px;
        }
    }

    .cards__link {
        position: absolute;
        bottom: 0;
        left: 0;
        width: 160px;
        height: 50px;
        border: none;
        cursor: pointer;

        display: flex;
        justify-content: center;
        align-items: center;

        font-weight: bold;
        font-size: 18px;
        line-height: 22px;
        text-align: center;

        color: $second-color;

        background: $first-color;

        transition: background-color 0.5s ease, border 1s ease;

        &:hover {
            box-sizing: border-box;
            background-color: $fourth-color;
            border: 1px solid $second-color;
        }
    }

    .cards__title-country {
        font-size: 9px;
        line-height: 11px;

        color: $color-country;
    }

    .cards__content-title {
        font-size: 18px;
        line-height: 22px;
        text-align: center;
        font-weight: bold;

        color: $second-color;
        text-align: left;

        margin: 0 0 20px 0;
    }

    .cards__paragraph-countries {
        font-size: 9px;
        line-height: 13px;
        margin: 0 0 15px 0;

        color: $color-countries;
    }

    .cards__paragraph-date {
        max-width: 150px;
        font-size: 9px;
        line-height: 11px;
        font-weight: bold;

        color: $second-color;
    }

    .cards__link-sall-out {
        width: 130px;
        height: 17px;
        border: none;
        display: flex;
        justify-content: center;
        align-items: center;
        cursor: pointer;

        margin:  0 0 56px 0;

        font-size: 9px;
        line-height: 11px;
        color: $fourth-color;

        background-color: $third-color ;
        border-radius: 3px;

        transition: transform 0.2s ease;

        &:hover {
            background-color: $first-color;
            color: $second-color;
            transform: scale(1.3);
        }
    }
    
</style>>
