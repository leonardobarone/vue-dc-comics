<template>
  <div class="container-fluid">
    <div class="footer-bottom container">
    <div class="left">
      <button class="btn">
        SIGN-UP NOW!
      </button>
    </div>
    <div class="right">
      <ul>
        <li>
          <a class="follow-us" href="#">
            FOLLOW US
          </a>
        </li>
        <li>
          <a href="#">
            <img src="../assets/img/footer-facebook.png" alt="">
          </a>
        </li>
        <li>
          <a href="#">
            <img src="../assets/img/footer-periscope.png" alt="">
          </a>
        </li>
        <li>
          <a href="#">
            <img src="../assets/img/footer-pinterest.png" alt="">
          </a>
        </li>
        <li>
          <a href="#">
            <img src="../assets/img/footer-twitter.png" alt="">
          </a>
        </li>
        <li>
          <a href="#">
            <img src="../assets/img/footer-youtube.png" alt="">
          </a>
        </li>
      </ul>
    </div>
  </div>
  </div>
</template>

<script>
export default {
  name: 'FooterBottom',
  props: {
    msg: String
  }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/common.scss';

.container-fluid {
  background-color: $main-color;
  padding: 1.25rem 0rem;
}


.container {
  @include misura-container;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1.25rem 0rem;
}

.btn {
  padding: .625rem;
  color: white;
  border: .0625rem solid $accent-color;
  background-color: transparent;
  cursor: pointer;
}



ul {
  display: flex;
  li {
    @include reset-list;
    margin-left: .625rem;
    .follow-us {
      font-size: 20px;
      font-weight: bold;
      line-height: 2.1875rem;
      margin-right: .625rem;
      @include reset-tag-a;
      color: $accent-color;
    }
    img {
      display: block;
    }
  }
}

  



</style>
