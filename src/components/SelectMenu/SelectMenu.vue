

<template>
  <div class="select-menu">
    <div class="select-menu__container">
        <select class="select-menu__list">
          <option class="select-menu__item">Страны</option>
          <option class="select-menu__item" value=”GR”>Green</option>
          <option class="select-menu__item" value=”YE”>Yellow</option>
          <option class="select-menu__item" value=”BL”>Black</option>
        </select>
        <select class="select-menu__list">
            <option class="select-menu__item">Даты</option>
            <option class="select-menu__item" value=”GR”>Green</option>
            <option class="select-menu__item" value=”YE”>Yellow</option>
            <option class="select-menu__item" value=”BL”>Black</option>
        </select>
    </div>
    <div class="select-menu__container">
      <div class="select-menu__styled-container">
        <select class="select-menu__list select-menu__list_bottom">
          <option class="select-menu__item">Тип путешествия</option>
          <option class="select-menu__item" value=”GR”>Green</option>
          <option class="select-menu__item" value=”YE”>Yellow</option>
          <option class="select-menu__item" value=”BL”>Black</option>
        </select>
      </div>
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
    }
  }
</script>

<style lang="scss">
    .select-menu {
      color: rgba(196, 196, 196, 0.3);
      height: 25%;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: flex-end;
    }

    .select-menu__container {
      position: relative;
    }

    .select-menu__list {
      width: 150px;
      height: 49px;
      outline: none;
      box-sizing: border-box;
      padding: 0 30px;

      background: $fourth-color;
      border-radius: 29.5px;

      -webkit-appearance: none;
      -moz-appearance: none;
      appearance: none;
      background: url('./Vector.png') 96% / 6% no-repeat #fff;
      background-position: 85% 50%;
      border: none;
      &::-ms-expand { 
        display: none;
        }
    }

    .select-menu__list.select-menu__list_bottom {
      width: 283px;
      background: url('./Vector.png') 96% / 3% no-repeat #fff;
    }

    .select-menu__item {
      background-color: $fourth-color;
      outline: none;
      border: none;
    }

    .select-menu__styled-container {
      background: #FFFFFF;
      border-radius: 29.5px;
      width: 283px;
      height: 80%;
    }
</style>>
