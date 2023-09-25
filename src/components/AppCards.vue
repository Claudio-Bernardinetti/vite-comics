<script>

export default {
  props: ['dcComics']
  }
  
</script>

<template>
    <div id="app_cards">
        <div v-for="(comic, index) in dcComics" :key="index">
            <img :src="comic.thumb" :alt="comic.series">
            <h2>{{ comic.series }}</h2>
            <p>{{ comic.type }}</p>
            <p>{{ comic.price }}</p>
        </div>
    </div>
</template>



<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

#app_header {
  
}
</style>