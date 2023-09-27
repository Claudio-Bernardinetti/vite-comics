<script>
    export default {
        name: 'Card',
        props: {
            comic: Object
        }
    }
</script>

<template>
    
    <div class="comic_item">
        <div class="image_container">
            <img class="comic_image" :src="comic.thumb" :alt="comic.series">
        </div>
        <div class="title_container justify-con">
            <h6 v-html="comic.series.replace('Knight', 'Knight<br>')"></h6> 
            <!-- <p>{{ comic.type }}</p>
            <p>{{ comic.price }}</p> -->
        </div>
    </div>
        
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

    .comic_item {
      
      margin: 0.5rem;

      .image_container {
        width: 100%;
        height: 130px;
        overflow: hidden;

        .comic_image {
          width: 130px;
          height: auto;
          object-fit: cover;
        }
      }

      .title_container {
        text-align: left;
        margin-top: 0.5rem;

        h6 {
          font-size: 50%;
          margin-top: 1rem;
          text-transform: uppercase;
        }
      }
    }
  
</style>


