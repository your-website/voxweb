<template>
    <form class="form">
        <h2 class="form__content-title">НЕМНОГО О ВАС</h2>
        <div class="form__container">
            <div class="form__fieldset">
                <label class="form__label" for="name">ИМЯ <span class="form__span form__span_color">*</span></label>
                <input class="form__input form__input_name" id="name" type="email" placeholder="Введите почту">
                <span class="form__error form__error_name"></span>
            </div>
            <div class="form__fieldset">
                <label class="form__label" for="tel">Телефон</label>
                <input class="form__input form__input_tel" id="tel" type="tel" placeholder="+7___ ___ __ __">
                <span class="form__error form__error_tel"></span>
            </div>
        </div>
        <h2 class="form__content-title form__content-title_width-travel">О ПУТЕШЕСТВИИ</h2>
        <div class="form__container">
            <div class="form__fieldset">
                <label class="form__label" for="country">КУДА И КОГДА ХОТИТЕ ПОЕХАТЬ? <span class="form__span form__span_color">*</span></label>
                <input class="form__input form__input_country" id="country" type="text" placeholder="Континент, страна или город">
                <span class="form__error form__error_country">Укажите континет, страну или город</span>
            </div>
            <div class="form__fieldset">
                <label class="form__label" for="date">КОГДА ?</label>
                <input class="form__input form__input_date" id="date" type="date" placeholder="Даты или временной интервал">
                <span class="form__error form__error_date"></span>
            </div>
        </div>
        <div class="form__container_checkbox">
            <h2 class="form__content-title form__content-title_width-contacts">УДОБНЫЙ СПОСОБ СВЯЗИ</h2>
            <h2 class="form__content-title form__content-title_width-about">ОТКУДА УЗНАЛИ О НАС</h2>
        </div>
        <div class="form__container_checkbox">
            <div class="form__container form__container_contacts">
                <div class="form__fieldset form__fieldset_contacts">
                    <label class="form__label" for="viber">VIBER</label>
                    <label class="form__label-checkbox">
                    <input class="form__checkbox" type="checkbox" name="viber"><span class="form__span_checkbox-big"></span></label>
                </div>
                <div class="form__fieldset form__fieldset_contacts">
                    <label class="form__label" for="WHATSAPP">WHATSAPP</label>
                    <label class="form__label-checkbox">
                    <input class="form__checkbox" type="checkbox" name="WHATSAPP"><span class="form__span_checkbox-big"></span></label>
                </div>
                <div class="form__fieldset form__fieldset_contacts">
                    <label class="form__label" for="post">ПОЧТА</label>
                    <label class="form__label-checkbox">
                    <input class="form__checkbox" type="checkbox" name="post"><span class="form__span_checkbox-big"></span></label>
                </div>
                <div class="form__fieldset form__fieldset_contacts">
                    <label class="form__label" for="tel">ТЕЛЕФОН</label>
                    <label class="form__label-checkbox">
                    <input class="form__checkbox" type="checkbox" name="tel"><span class="form__span_checkbox-big"></span></label>
                </div>
            </div>
            <div class="form__container form__container_contacts">
                <div class="form__fieldset form__fieldset_contacts">
                    <label class="form__label" for="internet">ИНТЕРНЕТ</label>
                    <label class="form__label-checkbox">
                    <input class="form__checkbox" type="checkbox" name="internet"><span class="form__span_checkbox-big"></span></label>
                </div>
                <div class="form__fieldset form__fieldset_contacts">
                    <label class="form__label form__label_position" for="friends">РЕКОМЕНДОВАЛИ ДРУЗЬЯ</label>
                    <label class="form__label-checkbox">
                    <input class="form__checkbox" type="checkbox" name="friends"><span class="form__span_checkbox-big"></span></label>
                </div>
                <div class="form__fieldset form__fieldset_contacts">
                    <label class="form__label" for="social">СОЦ. СЕТИ</label>
                    <label class="form__label-checkbox">
                    <input class="form__checkbox" type="checkbox" name="social"><span class="form__span_checkbox-big"></span></label>
                </div>
                <div class="form__fieldset form__fieldset_contacts">
                    <label class="form__label" for="know">УЖЕ ЕЗДИЛ</label>
                    <label class="form__label-checkbox">
                    <input class="form__checkbox" type="checkbox" name="know"><span class="form__span_checkbox-big"></span></label>
                </div>
            </div>
        </div>
        <div class="form__fieldset form__fieldset_bottom">
            <label class="form__label form__label_policy" for="tel">Получать свежие предложения по электронной почте</label>
            <label class="form__label-checkbox form__label-checkbox_size">
            <input class="form__checkbox" type="checkbox" name="know"><span class="form__span_checkbox-small"></span></label>
            <p class="cards__paragraph">Каждую неделю мы делаем для вас обзор лучших экспедиций, статей и лайфхаков для путешественников. Если вдруг вам не понравится, вы сможете отписаться в любой момент.</p>
        </div>
        <div class="form__fieldset form__fieldset_bottom">
            <label class="form__label form__label_policy" for="tel">С обработкой своих персональных данных согласен. <span class="form__span form__span_color">*</span></label>
            <label class="form__label-checkbox form__label-checkbox_size form__label-checkbox_color">
            <input class="form__checkbox form__checkbox_color" type="checkbox" name="know"><span class="form__span_checkbox-small"></span></label>
            <p class="cards__paragraph">Отправляя заявку я подтверждаю согласие с условиями Пользовательского соглашения</p>
        </div>
        <button class="form__button">ОТПРАВИТЬ</button>
    </form>
</template>

<script>
// const validator = require('validator');

  export default {
    components: {
    },
    data: function() {
        return {
        };
    },
    methods: {
        // validateTel: function() {
        //     if (validator.isMobilePhone(value, ['ru-RU'])) {

        //     } else {
                
        //     }
        // },
        // validateEmpty: function() {
        //     if (validator.isLength(value, {min:1, max: undefined})) {
        //     } else {
                
        //     }
        // }
    }
  }
</script>

<style lang="scss">
    .form__container_checkbox {
        display: flex;
        justify-content: space-between;

        @media screen and (max-width: 860px) {
            flex-direction: column;
        }

    }
    .form__label-checkbox {
        width: 40px;
        height: 40px;
        display: block;
        position: relative;
        background: #FFFFFF;
        border: 1px solid #E7E7E7;
        box-sizing: border-box;
        border-radius: 3px;
        cursor: pointer;
        overflow: hidden;
    }

    .form__label.form__label_position {
        max-width: 50px;
        text-align: center;
    }

    .form__label.form__label_policy {
        position: absolute;
        top: 3px;
        left: 25px;
    }

    .form__fieldset.form__fieldset_contacts {
        position: relative;
        margin-right: 40px;
        justify-content: flex-end;
    }

    .form__label-checkbox.form__label-checkbox_color {
        border: 1px solid $third-color;
    }

    .form__label-checkbox.form__label-checkbox_size {
        width: 15px;
        height: 15px;
    }
    .form__checkbox {
        display: none;
    }

    .form__checkbox:checked + .form__span_checkbox-big {
        position: absolute;
        top: 35%;
        left: 27%;
        width: 60px;
        height: 60px;
        background: url('../../assets/images/checkbox.png') no-repeat;
        cursor: pointer;
    }

    .form__checkbox:checked + .form__span_checkbox-small {
        position: absolute;
        top: 3px;
        left: 1px;
        width: 15px;
        height: 15px;
        background: url('../../assets/images/checkbox_small.png') no-repeat;
        cursor: pointer;
    }

    .form {
        max-width: 750px;

        @media screen and (max-width: 860px) {
            margin-left: 15%;
        }
        @media screen and (max-width: 525px) {
            margin-left: 0;
        }
    }

    .form__content-title {
        max-width: 87px;
        margin-bottom: 38px;

        font-size: 10px;
        line-height: 12px;
        padding-bottom: 3px;
        border-bottom: 2px solid $second-color;
        color: $second-color;
    }

    .form__content-title.form__content-title_width-travel {
        max-width: 94px;
    }

    .form__content-title.form__content-title_width-contacts {
        max-width: 138px;
    }

    .form__content-title.form__content-title_width-about {
        max-width: 124px;
    }

    .form__container {
        display: flex;
        margin-bottom: 35px;

        @media screen and (max-width: 860px) {
            flex-direction: column;
        }
    }

    .form__container.form__container_contacts {
        
        @media screen and (max-width: 860px) {
            flex-direction: row;
        }
    }

    .form__fieldset {
        position: relative;
        display: flex;
        flex-direction: column;
        margin-right: 20px;

        &:last-of-type {
            margin-right: 0;
        }

        @media screen and (max-width: 460px) {
            margin-right: 0;
        }
    }

    .form__label {
        margin-bottom: 8px;

        font-size: 10px;
        line-height: 12px;
        font-weight: bold;
        color: $second-color;
    }

    .form__input {
        width: 380px;
        height: 50px;
        padding-left: 30px;

        background: $fourth-color;
        border: 1px solid #E7E7E7;
        box-sizing: border-box;
        border-radius: 3px;

        @media screen and (max-width: 860px) {
            margin-bottom: 20px;
        }

        @media screen and (max-width: 460px) {
            width: 300px;
            height: 50px;
        }
    }

    .form__error {
        position: absolute;
        bottom: -17px;
        left: 0;
        font-size: 10px;
        line-height: 12px;

        color: $third-color;

        @media screen and (max-width: 860px) {
            bottom: 4px;
        }
    }

    .form__span_color {
        color: $third-color;
    }

    .form__button {
        width: 280px;
        height: 49px;
        border: none;
        cursor: pointer;

        background: $first-color;
        border-radius: 29.5px;

        transition: background-color 0.5s ease;

        &:hover {
            background-color: $button-hover;
        }
    }

    .cards__paragraph {
        font-size: 10px;
        line-height: 12px;

        color: $color-checkbox-paragraph;
    }
</style>>
