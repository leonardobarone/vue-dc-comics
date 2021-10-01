<template>
  <div class="container-fluid">
    <div class="section-blue container">

            <div class="prodotto">
                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                <h3>DIGITAL COMICS</h3>
            </div>

            <div class="prodotto">
                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                <h3>DIGITAL COMICS</h3>
            </div>

            <div class="prodotto">
                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                <h3>DIGITAL COMICS</h3>
            </div>

            <div class="prodotto">
                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                <h3>DIGITAL COMICS</h3>
            </div>

            <div class="prodotto">
                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                <h3>DIGITAL COMICS</h3>
            </div>

            <div class="prodotto">
                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                <h3>DIGITAL COMICS</h3>
            </div>

            <div class="prodotto">
                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                <h3>DIGITAL COMICS</h3>
            </div>
            
   

 
    </div>
  </div>
</template>

<script>
export default {
  name: 'SectionBlue',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/common.scss';
@import '../assets/style/variables.scss';

.container {
    display: flex;
    align-content: flex-start;
    flex-wrap: wrap;
    @include misura-container;
}

.container-fluid {
    background-color: $accent-color;

        .section-blue {
            padding: 25px;
        }

}

.prodotto {
    width: 20%;
    display: flex;
    align-items: center;
        img {
            width: 33px;
        }
}


</style>
