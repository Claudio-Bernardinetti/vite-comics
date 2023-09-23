<script>
import AppHeader from './components/AppHeader.vue';
import AppBlack from './components/AppBlack.vue';

export default {

  name: 'App',
  data() {
    return {

    }
  },
  components: {
    AppHeader,
    AppBlack,
    
}

}
</script>

<template>
  <AppHeader></AppHeader>
  <AppBlack></AppBlack>

</template>

<style lang="scss">
/* @use './assets/scss/app.scss'; */
</style>