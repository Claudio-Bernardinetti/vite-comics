<script>

export default {
  
}
</script>

<template>
 <div id="app_black">
    <div> Content goes here </div>
 </div>
    
</template>



<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

#app_black {
    display: flex;
    align-items: center;
    background-color: $comics_dark;
    height: 130px;
    padding-left: 15%;
    font-weight: bold;
    font-size: 120%;

    div {
        color: $comics_secondary;
    }
}

</style>