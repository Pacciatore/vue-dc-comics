<template>
  <div id="app">
    <HeaderComponent :navLi="headerNavLi" />
    <MainComponent />
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

import './components/fonts.css';

export default {
  name: 'App',
  data() {
    return {
      headerNavLi: [
        {
          text: 'Characters',
          active: false
        },
        {
          text: 'Comics',
          active: true
        },
        {
          text: 'Movies',
          active: false
        },
        {
          text: 'TV',
          active: false
        },
        {
          text: 'Games',
          active: false
        },
        {
          text: 'Collectibles',
          active: false
        },
        {
          text: 'Videos',
          active: false
        },
        {
          text: 'Fans',
          active: false
        },
        {
          text: 'News',
          active: false
        },
        {
          text: 'Shop',
          active: false
        },
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
