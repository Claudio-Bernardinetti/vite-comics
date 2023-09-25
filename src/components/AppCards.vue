<script>

export default {
  props: ['dcComics'],
  methods: {
    getImageUrl(props) {
      return new URL(`../../src/assets/img${props}.jpg`, import.meta.url).href;
    }
  }
}

  
</script>

<template>
    <div id="app_cards" class="d-flex flex-wrap">
        
        <div v-for="(comic, index) in dcComics.slice(0, 12)" :key="index">
            <img class="comic_image" :src="comic.thumb" :alt="comic.series">
            <div class="series_title">
                <h6 v-html="comic.series.replace('Knight', 'Knight<br>')"></h6> 
                <!-- <p>{{ comic.type }}</p>
                <p>{{ comic.price }}</p> -->
            </div>
        </div>
        <button class="px-5">LOAD MORE</button>
    </div>
</template>



<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

#app_cards {
    display: flex;
    justify-content: center;
    background-color: $comics_dark;
    color: $comics_secondary;
    padding-top: 2rem;
    padding-bottom: 2rem;

    .jumbotron {
       height: 300px;
       width: 100%;
        
    }

    .comic_image {
    width: 180px; 
    aspect-ratio: 1/1;
    object-fit: cover;
    margin: 0.5rem;
    
    }
    .series_title {
         text-transform: uppercase;
         margin-left: 0.5rem;
         
        h6 {
        font-size: 100%; 
        }
    font-size: 70%;
    }

    button{
        background-color: $comics_primary;
        color: $comics_secondary;
        height: 2rem;
        
    }
}
</style>