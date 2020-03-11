<template>
    <section class="travel">
        <h2 class="travel__content-title">ЗИМБАБВЕ</h2>
        <Cards></Cards>
    </section>
</template>

<script>
import Cards from '../Cards/Cards';
  export default {
    components: {
      Cards
    },
    data: function() {
        return {
        };
    },
   
  }
</script>

<style lang="scss">
    .travel {
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    .travel__content-title {
      margin: 46px 0;
      font-size: 36px;
      line-height: 43px;

      color: $second-color;
    }
    
</style>>
