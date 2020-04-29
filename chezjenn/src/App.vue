<template>
  <div id="app">
    <Navigation />
    <Welcome />
    <Showcase />
    <Footer />
  </div>
</template>

<script>
import Navigation from './components/Navigation.vue'
import Welcome from './components/Welcome.vue'
import Showcase from './components/Showcase.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Navigation,
    Welcome,
    Showcase,
    Footer
  }
}
</script>

<style>
  @import './assets/styles/styles.css';
</style>
