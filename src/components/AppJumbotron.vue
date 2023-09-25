<script>
export default {
  name: 'AppJumbotron',
  methods: {
    getImageUrl(name) {
      return new URL(`../../src/assets/img${name}.jpg`, import.meta.url).href;
    }
  }
};
</script>

<template>
 <div id="app_jumbotron">
    <img class="jumbotron" src="" alt="">
    <button class="px-5">CURRENT SERIES</button>
 </div>
    
</template>



<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

#app_jumbotron {
    background-image: url(../../../src/assets/img/jumbotron.jpg);
    height: 400px;
    overflow: hidden;
}

button {
    background-color: $comics_primary;
    color: $comics_secondary;
    position: absolute;
    top: 68%;
    left: 9%;
    font-size: 120%;
}

</style>