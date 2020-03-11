<template>
    <div @click='toggle' class="menu">
        <span class="menu__line menu__line_one"></span>
        <span class="menu__line menu__line_two"></span>
        <span class="menu__line menu__line_three"></span>
    </div>
</template>

<script>

  export default {
    data: function() {
        return {
        };
    },
    methods: {
      toggle: function() {
        const lineOne = document.querySelector('.menu__line_one');
        const lineTwo = document.querySelector('.menu__line_two');
        const lineThree = document.querySelector('.menu__line_three');

        lineOne.classList.toggle('menu__line_one-toggle');
        lineTwo.classList.toggle('menu__line_two-toggle');
        lineThree.classList.toggle('menu__line_three-toggle');
      }
    }
  }
</script>

<style lang="scss">

.menu {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-end;
  cursor: pointer;
}

.menu__input {
  display: flex;
  width: 35px;
  height: 30px;
  position: absolute;
  cursor: pointer;
  opacity: 0; /* hide input */
  z-index: 1; /* top of the menu */
}

.menu__line{
  width: 30px;
  height: 5px;
  margin-bottom: 4px;
  background: $second-color;
  border-radius: 4px;
  -webkit-transition: all .5s cubic-bezier(.08,.81,.87,.71);
  -moz-transition: all .5s cubic-bezier(.08,.81,.87,.71);
  -ms-transition: all .5s cubic-bezier(.08,.81,.87,.71);
  -o-transition: all .5s cubic-bezier(.08,.81,.87,.71);
  transition: all .5s cubic-bezier(.08,.81,.87,.71);
}

.menu__line_one {
  transform-origin: 4px 0px;
}

.menu__line_three {
  transform-origin: bottom right;
}

.menu__line.menu__line_one-toggle {
  background-color: $fourth-color;
  transform: rotate(45deg) translate(5px);
}
.menu__line.menu__line_two-toggle {
  background-color: $fourth-color;
  transform: rotate(495deg) translate(2px);   
}
.menu__line.menu__line_three-toggle {
  background-color: $fourth-color;
  transform: rotate(45deg);
  opacity: 0;
}
</style>>
