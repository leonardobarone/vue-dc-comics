<template>
  <div class="container-fluid">
    <div class="footer-top container">
      <div class="left">
        <div class="left-1">
          <h4>DC COMICS</h4>
          <ul>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
            <li>Videos</li>
            <li>News</li>
          </ul>
          <h4>SHOP</h4>
          <ul>
            <li>Shop DC</li>
            <li>Shop DC Collection</li>
          </ul>
        </div>
        <div class="left-2">
          <h4>DC</h4>
          <ul>
            <li>Terms Of Use</li>
            <li>Privacy policy (New)</li>
            <li>Ad Choices</li>
            <li>Advertising</li>
            <li>Jobs</li>
            <li>Subscriptions</li>
            <li>Talent Workshops</li>
            <li>CPSC Certificates</li>
            <li>Ratings</li>
            <li>Shop Help</li>
            <li>Contact Us</li>
          </ul>
        </div>
        <div class="left-3">
          <h4>SITES</h4>
          <ul>
            <li>DC</li>
            <li>MAD Magazine</li>
            <li>DC Kids</li>
            <li>DC Universe</li>
            <li>DC Power Visa</li>
          </ul>  
        </div>
      </div>
      <div class="right">
       
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
@import '../assets/style/common.scss';

.container-fluid {
  background-image: url("../assets/img/footer-bg.jpg");
  background-position: center;
  background-repeat: no-repeat;
  .container {
    @include misura-container;
    height: 100%;
    display: flex;
  }
}

.left {
  display: flex;
  width: 50%;
  color: white;
  padding: 40px 0px;
}

.left-1, .left-2, .left-3 {
  width: calc(100% / 3);
}

h4 {
  margin: 10px 0px 5px 0px;
}

ul {
  @include reset-list;
  li {
    color: gray;
  }
}

.right {
  width: 50%;
  background-image: url("../assets/img/dc-logo-bg.png");
  background-size: 80%;
  background-repeat: no-repeat;
  background-position: center;
}

</style>
