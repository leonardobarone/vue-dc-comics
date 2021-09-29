<template>
  <div class="container-fluid">
    <div class="footer-top container">
      <div class="left">

      </div>
      <div class="right">
        <!-- <img src="@/assets/img/dc-logo-bg.png" alt=""> -->
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FooterTop',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '@/assets/style/common.scss';

.container-fluid {
  background-image: url("../assets/img/footer-bg.jpg");
  background-position: center;
  background-repeat: no-repeat;
  height: 200px;
}

.container {
  @include misura-container;
}
.left img {
  width: 300px;
}
</style>
