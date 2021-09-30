<template>
    <div class="container-fluid">
        <div class="container">
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
  props: ['card'],
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



</style>
