<script>

export default {
  
}
</script>

<template>
    <header id="app_header" class="text-center">

     
      <nav class="navbar navbar-expand justify-content-center">
          <div class="nav navbar-nav">
              <a class="nav-item nav-link" href="#" aria-current="page">Home <span class="visually-hidden">(current)</span></a>
              <a class="nav-item nav-link" href="#">About</a>
              <a class="nav-item nav-link active-item"  href="#">Products</a>
              <a class="nav-item nav-link" href="#">Contacts</a>

          </div>
      </nav>

    </header>
    <!-- /#app_header -->
</template>



<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

#app_header {
  background-color: $comics_light;
  a.active-item {
    background-color: $comics_secondary;
  }

}
</style>