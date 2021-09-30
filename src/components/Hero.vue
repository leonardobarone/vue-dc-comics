<template>
    <div class="hero">
        <div class="container">
            <a class="button" href="#">CURRENT SERIES</a>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Hero',
  props: {
    msg: String
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import '../assets/style/common.scss';
@import '../assets/style/variables.scss';

.hero {
    position: relative;
    @include bg-custom;
    height: 300px;
    background-image: url("../assets/img/jumbotron.jpg");
}

.container {
    @include misura-container;
}


a.button {
    position: absolute;
    bottom: -20px;
    font-weight: bold;
    @include reset-tag-a;
    color: white;
    font-size: 20px;
    padding: 10px 15px;
    background-color: $accent-color;
}

</style>
