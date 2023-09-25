<script>
export default {
  name: 'AppJumbotron',
};
</script>

<template>
 <div id="app_jumbotron">
    <img class="jumbotron" src="../../../src/assets/img/jumbotron.jpg" alt="">
 </div>
    
</template>



<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

#app_jumbotron {
    height: 400px;
    overflow: hidden;
}

</style>