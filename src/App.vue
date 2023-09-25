<script>
import AppHeader from './components/AppHeader.vue';
import AppBlack from './components/AppBlack.vue';
import AppBlue from './components/AppBlue.vue';
import AppFooterTop from './components/AppFooterTop.vue';
import AppFooterBottom from './components/AppFooterBottom.vue';
import AppCards from './components/AppCards.vue'
import dcComics from '../../vite-comics/dcComics.json';

export default {

  components: {
    AppHeader,
    AppBlack,
    AppBlue,
    AppFooterTop,
    AppFooterBottom,
    AppCards,
  },

    data() {
      return {
        dcComics
      }
    }

}
</script>

<template>
  <AppHeader></AppHeader>
  <AppBlack></AppBlack>
  <AppBlue></AppBlue>
  <AppFooterTop></AppFooterTop>
  <AppFooterBottom></AppFooterBottom>
  
  <div>
    <AppCards :dcComics="dcComics" />
  </div>
  
  

</template>

<style lang="scss">
/* @use './assets/scss/app.scss'; */
</style>