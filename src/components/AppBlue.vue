<script>

export default {
  
}
</script>

<template>
 <div id="app_blue" class="d-flex flex-grow align-items-center justify-content-between">
    <div class="card_digilal">
        <img src="../../../src/assets/img/buy-comics-digital-comics.png" alt="">
        <div class="text">DIGITAL COMICS</div>
    </div>
    <div class="card_merchandise">
        <img src="../../../src/assets/img/buy-comics-merchandise.png" alt="">
        <div class="text">DC MERCHANDISE</div>
    </div>
    <div class="card_subscription">
        <img src="../../../src/assets/img/buy-comics-subscriptions.png" alt="">
        <div class="text">SUBSCRIPTION</div>
    </div>
    <div class="card_locator">
        <img src="../../../src/assets/img/buy-comics-shop-locator.png" alt="">
        <div class="text">COMIC SHOP LOCATOR</div>
    </div>
    <div class="card_visa">
        <img src="../../../src/assets/img/buy-dc-power-visa.svg" alt="">
        <div class="text">DC POWER VISA</div>
    </div>
    
 </div>
    
</template>



<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

#app_blue {
    background-color: $comics_primary;
    // height: 150px;
    padding-left: 13%;
    
    img {
        width: 20%;
    }

    div {
        display: flex;
        align-items: center;
        color: $comics_secondary;
        font-size: 90%;
        padding-top: 1.5rem;
        padding-bottom: 1.5rem;
        padding-left: 0.5rem;
       
    }

    .card_locator {

        img {
            width:10%;
        }
    }

    .card_visa {

        img {
            width:10%;
        }
    }
}

</style>