<script>

export default {
  name: 'AppHeader',
  
}
</script>

<template>
    <header id="app_header">

      <!-- <nav class="navbar navbar-expand justify-content-center align-items-center"> -->
          
            <div class="nav_img">
              <img src="../../../src/assets/img/dc-logo.png" width="60px" alt="">
            </div>
            <div class="nav_tags">
                <div><a href="#">CHARACTERS</a></div>
                <div class="active"><a  href="#">COMICS</a></div>
                <div><a href="#">MOVIES</a></div>
                <div><a href="#">TV</a></div>
                <div><a href="#">GAMES</a></div>
                <div><a href="#">COLLECTIBLES</a></div>
                <div><a href="#">VIDEOS</a></div>
                <div><a href="#">FANS</a></div>
                <div><a href="#">NEWS</a></div>
                <div><a href="#">SHOP</a></div>
            </div>
          
      <!-- </nav> -->

    </header>
    <!-- /#app_header -->
</template>



<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

#app_header {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  align-items: center;
  background-color: $comics_secondary;
  font-weight: bold;
  font-size: 70%;

  .nav_img {
     padding: 1rem;
  }
  .nav_tags  {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    
    .active {
      
      border-bottom: 4px solid $comics_primary;
      
      a {
      color: $comics_primary;
      }

    }

  }
  .nav_tags div {
    margin-left: 1rem;
    padding-top: 2.2rem;
    padding-bottom: 2.2rem;

  }

  a {
    text-decoration: none;
    color: $comics_dark;
  }

}
</style>