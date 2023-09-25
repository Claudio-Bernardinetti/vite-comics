<script>

export default {
  props: ['dcComics']
  }
  
</script>

<template>
    <div id="app_cards" class="d-flex flex-wrap">
        <div v-for="(comic, index) in dcComics.slice(0, 12)" :key="index">
            <img class="comic_image" :src="comic.thumb" :alt="comic.series">
            <div class="series_title">
                <h6 v-html="comic.series.replace('Knight', 'Knight<br>')"></h6> 
                <p>{{ comic.type }}</p>
                <p>{{ comic.price }}</p>
            </div>
        </div>
    </div>
</template>



<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

#app_cards {
    display: flex;
    justify-content: center;
    background-color: $comics_dark;
    color: $comics_secondary;

.comic_image {
  width: 180px; 
  aspect-ratio: 1/1;
  object-fit: cover;
  margin: 0.2rem; 
}
.series_title {
    h6 {
       font-size: 120%; 
    }
   font-size: 70%;
}
}
</style>