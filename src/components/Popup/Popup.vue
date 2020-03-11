<template>
    <header class="header">
      <Menu @click.native="toggle" class="menu_header"></Menu>
      <nav>
        <ul>
          <li></li>
          <li></li>
          <li></li>
          <li></li>
        </ul>
      </nav>
    </header>
</template>

<script>
import Menu from '../Menu/Menu';
  export default {
    components: {
      Menu
    },
    data: function() {
        return {
          isActive: false,
        };
    },
    methods: {
      toggle: function() {
        this.isActive = !this.isActive
        alert(this.isActive)
      }
    }
  }
</script>

<style lang="scss">
   
</style>>
