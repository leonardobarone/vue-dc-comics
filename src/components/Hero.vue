<template>
    <div class="hero" :style="`background-image: url(${imgHero})`">
        <div class="container">
           
        </div>
    </div>
</template>

<script>
export default {
  name: 'Hero',
  props: {
    imgHero: String
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import '../assets/style/common.scss';
@import '../assets/style/variables.scss';

.hero {
    @include bg-custom;
    height: 300px;
}

.container {
    @include misura-container;
}



</style>
