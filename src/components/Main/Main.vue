
<template>
    <main class="main">
      <Travel></Travel>
      <Buy></Buy>
    </main>
</template>

<script>
import Travel from '../Travel/Travel'
import Buy from '../Buy/Buy';
  export default {
    components: {
      Travel,
      Buy
    },
    data: function() {
        return {
          contentTitle: ['Day', 'Week', 'Month', 'Year'],
        };
    },
    
  }
</script>

<style lang="scss">
    @font-face {
        src: url('../../styles/MuseoSansCyrl/MuseoSansCyrl_0.otf');
        font-family: 'Museo Sans Cyrl';
    }
    main {
        font-family: Museo Sans Cyrl, Arial, sans-serif;
        justify-content: space-around;
        background-color: #fff;

        @media screen and (max-width: 1024px) {
          flex-direction: column;
        }
    }
</style>>
