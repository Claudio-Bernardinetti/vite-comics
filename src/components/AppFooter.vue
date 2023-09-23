<script>

export default {
  
}
</script>

<template>
 <div id="app_footer" class="d-flex flex-wrap justify-content-around align-items-center">

    <div class="footer_left">
        <button>SING-UP NOW!</button>
    </div>

    <div class="footer_right d-flex flex-wrap align-items-center">

        <div class="text">FOLLOW US</div>
        <div><img src="../../../src/assets/img/footer-facebook.png" alt=""></div>
        <div><img src="../../../src/assets/img/footer-periscope.png" alt=""></div>
        <div><img src="../../../src/assets/img/footer-pinterest.png" alt=""></div>
        <div><img src="../../../src/assets/img/footer-twitter.png" alt=""></div>
        <div><img src="../../../src/assets/img/footer-youtube.png" alt=""></div>

    </div>
    
 </div>
    
</template>



<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

#app_footer {
  background-color: $comics_dark_secondary;
  // height: 110px;
  width: 100%;
  position: absolute;
  bottom: 1;

  button{
    background: $comics_dark_secondary;
    color: $comics_secondary;
    padding: 0.5rem;
    border: 3px solid $comics_primary ;
  }

  .footer_right {
    padding: 1rem;
    div {
        padding: 0.5rem;
    }
  }

  .text {
    color: $comics_primary;
    font-weight: bold;
    font-size: 110%;
  }

}

</style>