<script>

export default {
  props: ['dcComics'],
  
}

</script>

<template>
  <div id="app_cards" >
    <div class="comic_container d-flex flex-wrap">
      <div v-for="(comic, index) in dcComics.slice(0, 12)" :key="index" class="comic_item">
        <div class="image_container">
          <img class="comic_image" :src="comic.thumb" :alt="comic.series">
        </div>
        <div class="title_container justify-con">
          <h6 v-html="comic.series.replace('Knight', 'Knight<br>')"></h6> 
          <!-- <p>{{ comic.type }}</p>
          <p>{{ comic.price }}</p> -->
        </div>
      </div>
    </div>
    <button class="px-5">LOAD MORE</button>
  </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

#app_cards {
  display: flex;
  flex-wrap: wrap; 
  justify-content: space-around;
  background-color: $comics_dark;
  color: $comics_secondary;
  padding-top: 2rem;
  padding-bottom: 2rem;

  .comic_container {
    display: flex;
    flex-wrap: wrap;
    margin: 0.5rem;

    .comic_item {
      width: calc(100% / 6 - 1rem);
      margin: 0.5rem;

      .image_container {
        width: 100%;
        height: 180px;
        overflow: hidden;

        .comic_image {
          width: 100%;
          height: auto;
          object-fit: cover;
        }
      }

      .title_container {
        text-align: left;
        margin-top: 0.5rem;

        h6 {
          font-size: 70%;
          margin-top: 1rem;
          text-transform: uppercase;
        }
      }
    }
  }

  button {
    background-color: $comics_primary;
    color: $comics_secondary;
    height: 2rem;
  }
}
</style>

