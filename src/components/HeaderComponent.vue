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
          <li v-for="navElement in navLi" :key="navElement" class="nav-item item fs-5">
            <a href="#" @click="setActive(navElement)" class="nav-link" :class="{active : activeIndex === navElement}">
              {{ navElement }}</a>
          </li>
        </ul>

      </nav>

    </div>

  </header>
</template>


<script>
export default {
  name: 'HeaderComponent',
  props: {
    navLi: Array,
  },
  data() {
    return {
      activeIndex: 'Comics'
    }
  },
  methods: {
    setActive(navElement) {
      return this.activeIndex = navElement
    }
  }
}
</script>


<style scoped lang="scss">
// Import variabili
@import '@/components/style/variables.scss';

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

  position: relative;

  &:hover {
    color: $tr-dc-blue;
  }

  &.active {
    color: $tr-dc-blue;
  }

  &.active::after {
    content: '';
    position: absolute;
    left: 0;
    bottom: -41px;

    width: 100%;
    height: 5px;
    background-color: $tr-dc-blue;
  }

}
</style>
