<script>

export default {
  name: 'AppFooterTop',
  
}
</script>

<template>
 <div id="app_footer_top">
    <div class="d-flex flex-wrap justify-content-around align-items-center p-3">
        <div class="text d-flex flex-wrap">
           <div>DC COMICS
             <ul>
                <li>Characters</li>
                <li>Comics</li>
                <li>Movies</li>
                <li>TV</li>
                <li>Games</li>
                <li>Videos</li>
                <li>News</li>
             </ul>
            <div>SHOP</div>
             <ul>
                <li>Shop DC</li>
                <li>Shop DC Collectibles</li>
             </ul>
           </div>
           <div>DC
            <ul>
                <li>Terms Of Use</li>
                <li>Privacy policy(New)</li>
                <li>Ad Choices</li>
                <li>Advertising</li>
                <li>Job</li>
                <li>Subscriptions</li>
                <li>Talent Workshops</li>
                <li>CPSC Certificates</li>
                <li>Ratings</li>
                <li>Shop Help</li>
                <li>Contact Us</li>
            </ul>
           </div>
           <div>SITES
            <ul>
                <li>DC</li>
                <li>MAD Magazine</li>
                <li>DC Kids</li>
                <li>DC Universe</li>
                <li>DC Power Visa</li>
            </ul>
           </div> 
        </div>
        <div class="img"><img src="../../src/assets/img/dc-logo-bg.png" width="60%" alt=""></div>
    </div>
    
 </div>
    
</template>



<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

#app_footer_top {
  background-image: url(../../../src/assets/img/footer-bg.jpg);
  position: relative; 
 
  
  div{
    color: $comics_secondary;
  }

  .text{

    div {
    padding-right: 1.5rem;
    font-weight: bold;
    font-size: 110%;
    }

    ul {
        list-style-type: none;
        color: $comics_light ;
        margin-left: -32px;
        padding-top: 1rem;
        font-weight: normal;
        font-size: 70%;
    }

  }
    .img { 
       margin-top: -8%;
       margin-bottom: -8%;
    }
}

</style>