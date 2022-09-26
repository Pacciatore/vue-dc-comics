<template>
  <div id="app">
    <HeaderComponent :navLi="headerNavLi" />
    <MainComponent :currentSeries="currentComics" />
    <FooterComponent />
  </div>
</template>

<script>
// Import bootstrap library
import 'bootstrap/dist/css/bootstrap.css'

// Import components
import HeaderComponent from './components/HeaderComponent.vue'
import MainComponent from './components/MainComponent.vue';
import FooterComponent from './components/FooterComponent.vue';

// Import data
import currentComics from '@/data/dc-comics'

// Import page font
import '@/assets/style/fonts.css';

export default {
  name: 'App',
  data() {
    return {
      currentComics,
      headerNavLi: [
        'Characters',
        'Comics',
        'Movies',
        'TV',
        'Games',
        'Collectibles',
        'Videos',
        'Fans',
        'News',
        'Shop'
      ]
    }
  },
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Teko', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
