<template>
  <div id="app">
    <Header />
    <Hero />
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
import Hero from './components/Hero.vue'

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    SectionBlue,
    SectionBlack,
    FooterTop,
    FooterBottom
  },
}
</script>

<style lang="scss">
  @import './assets/style/common.scss';
</style>
