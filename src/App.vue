<script>
import AppHeader from './components/AppHeader.vue';
import AppBlack from './components/AppBlack.vue';
import AppBlue from './components/AppBlue.vue';

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
    
}

}
</script>

<template>
  <AppHeader></AppHeader>
  <AppBlack></AppBlack>
  <AppBlue></AppBlue>

</template>

<style lang="scss">
/* @use './assets/scss/app.scss'; */
</style>