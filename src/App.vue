<script>
import AppHeader from './components/AppHeader.vue';
import AppBlack from './components/AppBlack.vue';
import AppBlue from './components/AppBlue.vue';
import AppFooterTop from './components/AppFooterTop.vue';
import AppFooterBottom from './components/AppFooterBottom.vue';

export default {

  name: 'App',
  data() {
    return {

    }
  },
  components: {
    AppHeader,
    AppBlack,
    AppBlue,
    AppFooterTop,
    AppFooterBottom,
}

}
</script>

<template>
  <AppHeader></AppHeader>
  <AppBlack></AppBlack>
  <AppBlue></AppBlue>
  <AppFooterTop></AppFooterTop>
  <AppFooterBottom></AppFooterBottom>

</template>

<style lang="scss">
/* @use './assets/scss/app.scss'; */
</style>