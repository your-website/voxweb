<template>
    <section class="buy">
        <h2 class="buy__content-title">Заявка на подбор путешествия</h2>
        <Form></Form>
    </section>
</template>

<script>
import Form from '../Form/Form';

  export default {
    components: {
        Form
    },
    data: function() {
        return {
        };
    },
   
  }
</script>

<style lang="scss">
    .buy {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin-bottom: 100px;

      @media screen and (max-width: 525px) {
            margin-left: 4px;
        }
    }
    .buy-title {
      margin: 0 0 70px 0;
      font-size: 36px;
      line-height: 43px;

      color: $second-color;
    }
    
</style>>
