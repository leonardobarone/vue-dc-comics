<template>
    <div class="container-fluid">
        <div class="container">
            <a class="button" href="#">CURRENT SERIES</a>
            <Card :card="eroe" v-for="(eroe, index) in eroi" :key="index" />
        </div>
        <div class="container-2">
            <div class="button">
                <a href="#">
                    LOAD MORE
                </a>
            </div>
        </div>
    </div>
</template>

<script>
import Card from '../components/Card.vue'
import json from '../assets/materiale/dc-comics.json'

export default {
  name: 'SectionBlack',
  components: {
      Card,
  },
// SEMBREREBBE INUTILE
// props: ['card'],
  data() {
      return {
          eroi: json
      }
}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import '../assets/style/common.scss';
@import '../assets/style/variables.scss';

.container-fluid {
    background-color: $main-color;
}

.container {
    position: relative;
    padding: 3.5rem 0rem;
    @include misura-container;
    color: white;
    display: flex;
    flex-wrap: wrap;
     
}

.container-2 {
    @include misura-container;
    text-align: center;
    padding: 10px;
    .button { 
        margin-bottom: 2.5rem;
        a {
        font-weight: bold;
        padding: 7px 23px;
        background-color: $accent-color;
        @include reset-tag-a;
        color: white;
    }

}
}


a.button {
    position: absolute;
    top: -25px;
    font-weight: bold;
    @include reset-tag-a;
    color: white;
    font-size: 20px;
    padding: 10px 15px;
    background-color: $accent-color;
}



</style>
