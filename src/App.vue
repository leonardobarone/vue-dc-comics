<template>
  <div id="app">
    <Header />
    <SectionBlack />
    <SectionBlue />
    <footer>
      <FooterTop />
      <FooterBottom />
    </footer>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import SectionBlue from './components/SectionBlue.vue'
import FooterTop from './components/FooterTop.vue'
import FooterBottom from './components/FooterBottom.vue'
import SectionBlack from './components/SectionBlack.vue'

export default {
  name: 'App',
  components: {
    Header,
    SectionBlack,
    SectionBlue,
    FooterTop,
    FooterBottom
  },
}
</script>

<style lang="scss">
  @import '@/assets/style/common.scss';
</style>
