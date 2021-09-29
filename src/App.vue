<template>
  <div id="app">
    <Header />
    <footer>
      <FooterTop />
      <FooterBottom />
    </footer>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import FooterTop from '@/components/FooterTop.vue'
import FooterBottom from '@/components/FooterBottom.vue'

export default {
  name: 'App',
  components: {
    Header,
    FooterTop,
    FooterBottom
  },
}
</script>

<style lang="scss">
  @import '@/assets/style/common.scss';
</style>
