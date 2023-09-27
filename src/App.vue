<script>
import AppHeader from './components/AppHeader.vue';
import AppJumbotron from './components/AppJumbotron.vue';
import AppBlue from './components/AppBlue.vue';
import AppFooterTop from './components/AppFooterTop.vue';
import AppFooterBottom from './components/AppFooterBottom.vue';
import AppCards from './components/AppCards.vue';

import dcComics from '../../vite-comics/dcComics.json';

export default {

  components: {
    AppHeader,
    AppJumbotron,
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
  <AppJumbotron></AppJumbotron>
  <div>
    <AppCards :dcComics="dcComics" />
    
  </div>
  <AppBlue></AppBlue>
  <AppFooterTop></AppFooterTop>
  <AppFooterBottom></AppFooterBottom>
  
  
  

</template>

<style lang="scss">
/* @use './assets/scss/app.scss'; */
</style>