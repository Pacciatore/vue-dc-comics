<template>
  <header>

    <div class="container py-4">


      <nav class="navbar navbar-expand-lg justify-content-between">

        <a class="img-container navbar-brand" href="#">
          <img src="../assets/img/dc-logo.png" alt="dc-logo">
        </a>

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

.nav-link {
  color: $tr-dc-black;
  font-weight: 500;
  text-transform: uppercase;
}

.nav-link:hover {
  color: $tr-dc-blue;
}

.nav-link.active {
  // Da aggiungere in una variabile tr-dc-blue
  color: $tr-dc-blue;
  border-bottom: 5px solid $tr-dc-blue;
}
</style>
