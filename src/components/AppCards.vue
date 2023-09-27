<script>
import Card from './Card.vue';

export default {
  name: 'AppCards',
  props: ['dcComics'],
  components: {
    Card,
  },
  
}

</script>

<template>
<div id="app_cards">
  <div class="d-flex flex-wrap justify-content-start">
    <div class="p-2" v-for="(comic, index) in dcComics.slice(0, 12)" :key="index">
      <Card :comic="comic" />
    </div>
  </div>
  <div class="d-flex justify-content-center py-2">
    <button class="px-5">LOAD MORE</button> 
  </div> 
</div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

button {
    background-color: $comics_primary;
    color: $comics_secondary;
    height: 2rem;
  }


</style>

