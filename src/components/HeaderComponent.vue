<template>
  <header>

    <div class="container">

      <!-- Barra di navigazione -->
      <nav class="navbar navbar-expand-lg justify-content-between">

        <!-- Logo della pagina -->
        <a class="img-container navbar-brand" href="#">
          <img src="../assets/img/dc-logo.png" alt="dc-logo">
        </a>

        <!-- Elementi di navigazione -->
        <ul class="navbar-nav">
          <li class="nav-item item fs-5"> <a href="#" class="nav-link">Characters</a></li>
          <li class="nav-item item fs-5"> <a href="#" class="nav-link active">Comics</a></li>
          <li class="nav-item item fs-5"> <a href="#" class="nav-link">Movies</a></li>
          <li class="nav-item item fs-5"> <a href="#" class="nav-link">TV</a></li>
          <li class="nav-item item fs-5"> <a href="#" class="nav-link">Games</a></li>
          <li class="nav-item item fs-5"> <a href="#" class="nav-link">Collectibles</a></li>
          <li class="nav-item item fs-5"> <a href="#" class="nav-link">Videos</a></li>
          <li class="nav-item item fs-5"> <a href="#" class="nav-link">Fans</a></li>
          <li class="nav-item item fs-5"> <a href="#" class="nav-link">News</a></li>
          <li class="nav-item item fs-5"> <a href="#" class="nav-link">Shop</a></li>
        </ul>

      </nav>

    </div>

  </header>
</template>


<script>
export default {
  name: 'HeaderComponent',
}
</script>


<style scoped lang="scss">
// Import variabili
@import './variables.scss';

.navbar-brand {


  transition: all 0.25s;

  &:hover {
    filter: grayscale(1) contrast(5)
  }

}

.nav-link {
  color: $tr-dc-black;
  font-weight: 500;
  text-transform: uppercase;

  &:hover {
    color: $tr-dc-blue;
  }

  &.active {
    color: $tr-dc-blue;
    border-bottom: 5px solid $tr-dc-blue;
  }


}
</style>
