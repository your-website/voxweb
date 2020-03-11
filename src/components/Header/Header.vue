<template>
    <header class="header">
      <Menu @click.native="toggle" class="menu_header"></Menu>
      <div class="header__container">
        <SelectMenu></SelectMenu>
        <button class="header__button">Найти</button>
        <nav class="header__nav">
          <ul class="header__list">
            <li class="header__item"><a class="header__link" href="">ПУТЕШЕСТВИЯ</a></li>
            <li class="header__item"><a class="header__link" href="">О НАС</a></li>
            <li class="header__item"><a class="header__link" href="">ОТЗЫВЫ</a></li>
            <li class="header__item"><a class="header__link" href="">БЛОГ</a></li>
          </ul> 
        </nav>
        <a class="header__link header__link_tel" href="tel:+7 (495) 123-45-67">+7 (495) 123-45-67</a>
        <button class="header__button">ПОДБЕРИТЕ МНЕ ТУР</button>
      </div>
    </header>
</template>

<script>
import Menu from '../Menu/Menu';
import SelectMenu from '../SelectMenu/SelectMenu';
  export default {
    components: {
      Menu,
      SelectMenu
    },
    data: function() {
        return {
          isActive: false,
        };
    },
    methods: {
      toggle: function() {
        this.isActive = !this.isActive
        const popUp = document.querySelector('.header__container');
        popUp.classList.toggle('header__container_translate-x');
      }
    }
  }
</script>

<style lang="scss">
    @font-face {
        src: url('../../styles/MuseoSansCyrl/MuseoSansCyrl_0.otf');
        font-family: 'Museo Sans Cyrl';
    }

    .header {
      font-family: Museo Sans Cyrl, Arial, sans-serif;
      position: relative;
      display: flex;
      justify-content: flex-end;
      height: 70px;
      background-color: $first-color;
      overflow-x: hidden;

    }

    .menu_header {
      margin-right: 23px;
      z-index: 3;
    }

    .header__container {
      position: fixed;
      top: 0;
      right: 0;

      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: space-between;

      background-color: $first-color;
      height: 100vh;
      width: 530px;
      transform: translateX(530px);
      transition: transform 0.7s ease;
      z-index: 2;
      @media screen and (max-width: 660px) {
        width: 100%;
          transform: translateX(100%);
        }
    }

    .header__container.header__container_translate-x {
      transform: translateX(0);
    }

    .header__button {
      width: 280px;
      height: 49px;
      cursor: pointer;

      border: 1px solid $second-color;
      box-sizing: border-box;
      border-radius: 29.5px;

      background-color: transparent;

      font-size: 12px;
      line-height: 14px;

      color: $second-color;
      transition: color 0.3s ease, background-color 0.3s ease;

      &:hover {
        color: $fourth-color;
        background-color: $color-hover;
      }
    }

    .header__nav {

    }

    .header__list {

    }

    .header__item {
      list-style-type: none;

      
    }

    .header__link {
      text-decoration: none;
      font-weight: bold;
      font-size: 18px;
      line-height: 22px;
      letter-spacing: 0.1em;

      color: $second-color;

      &:hover {
        opacity: 0.7;
        color: $color-hover;
      }
    }

    .header__link.header__link_tel {
      font-style: normal;
      font-weight: bold;
      font-size: 24px;
      line-height: 29px;
      letter-spacing: 0.1em;

      &:hover {
        opacity: 0.9;
        color: $color-hover-tel;
      }
    }
</style>>
