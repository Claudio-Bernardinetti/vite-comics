<script>
import AppHeader from './components/AppHeader.vue';
import AppBlack from './components/AppBlack.vue';
import AppBlue from './components/AppBlue.vue';
import AppMain from './components/AppMain.vue';


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
    AppMain,
    
}

}
</script>

<template>
  <AppHeader></AppHeader>
  <AppBlack></AppBlack>
  <AppBlue></AppBlue>
  <AppMain></AppMain>

</template>

<style lang="scss">
/* @use './assets/scss/app.scss'; */
</style>