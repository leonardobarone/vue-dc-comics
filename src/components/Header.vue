<template>
  <header>
    <div class="container">
      <div class="logo">
        <img src="@/assets/img/dc-logo.png" alt="">
      </div>
      <nav>
        <ul>
          <li v-for="(link, index) in links" :key="index">
            <a :href="link.connection">
              {{ link.text.toUpperCase() }}
            </a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  props: {
    msg: String
  },
  data () {
    return {
      links: [
        {
          "text": "characters",
          "state": false,
          "connection": "#"
        },
        {
          "text": "comics",
          "state": false,
          "connection": "#"
        },
        {
          "text": "movies",
          "state": false,
          "connection": "#"
        },
        {
          "text": "tv",
          "state": false,
          "connection": "#"
        },
        {
          "text": "games",
          "state": false,
          "connection": "#"
        },
        {
          "text": "collectibles",
          "state": false,
          "connection": "#"
        },
        {
          "text": "videos",
          "state": false,
          "connection": "#"
        },
        {
          "text": "fans",
          "state": false,
          "connection": "#"
        },
        {
          "text": "news",
          "state": false,
          "connection": "#"
        },
        {
          "text": "shop",
          "state": false,
          "connection": "#"
        },
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

@import '@/assets/style/bootstrap.scss';
@import '@/assets/style/variables.scss';
  
  .container {
    border: 1px solid black;
    display: flex;
    justify-content: space-between;
    align-items: center;
    
    .logo img {
      width: 3.125rem;
      display: block;
    }

    ul {
      display: flex;
    }

    a {
      color: $text-header;
      font-weight: bold;
      margin-left: 10px;
      display: inline-block;
      height: 4.125rem;
      line-height: 4.125rem;
    }
  
  }


</style>
