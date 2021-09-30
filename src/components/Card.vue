<template>
    
            <div class="eroe">
                <img :src="card.thumb" alt="">
                <h5>{{card.series.toUpperCase()}}</h5>
            </div>
    
</template>

<script>
export default {
  name: 'Card',
  props: ['card']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import '../assets/style/common.scss';
@import '../assets/style/variables.scss';

.eroe {
         padding: .625rem;
         width: calc(100% / 6);
         img {
             object-fit: cover;
             object-position: top;
             width: 9.375rem;
             height: 9.375rem;
         }
         h5 {
             color: white;
             margin-top: .3125rem ;
         }
     }



</style>
