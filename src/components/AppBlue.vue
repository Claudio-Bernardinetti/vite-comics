<script>
export default {
  name: 'AppBlue',

  data(){
    return{
        cards: [
            {
                img: '../../../src/assets/img/buy-comics-digital-comics.png',
                text: 'DIGITAL COMICS',
                width: '20%'
            },
            {
                img: '../../../src/assets/img/buy-comics-merchandise.png',
                text: 'DC MERCHANDISE',
                width: '20%'
            },
            {
                img: '../../../src/assets/img/buy-comics-subscriptions.png',
                text: 'SUBSCRIPTION',
                width: '20%'
            },
            {
                img: '../../../src/assets/img/buy-comics-shop-locator.png',
                text: 'COMIC SHOP LOCATOR',
                width: '12%'
            },
            {
                img: '../../../src/assets/img/buy-dc-power-visa.svg',
                text: 'DC POWER VISA',
                width: '12%'
            },
        ]
    }
  }
};
</script>

<template>
 <div id="app_blue" class="d-flex  flex-wrap align-items-center justify-content-between">
    <div class="card_digilal" v-for="(card, index) in cards" :key="index">
        <img :src="card.img" :style="{ width: card.width }" alt="">
        <div class="text">{{card.text}}</div>
    </div>
    <!-- <div class="card_merchandise">
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
    </div> -->
    
 </div>
    
</template>



<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

#app_blue {
    background-color: $comics_primary;

    div {
        display: flex;
        align-items: center;
        color: $comics_secondary;
        font-size: 90%;
        padding-top: 1.5rem;
        padding-bottom: 1.5rem;
        
    }

    .text{
        padding-left: 0.2rem;
    }
}

</style>