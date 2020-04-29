<template>
  <div id="app">
    <Navigation />
    <Welcome />
    <Showcase />
  </div>
</template>

<script>
import Navigation from './components/Navigation.vue'
import Welcome from './components/Welcome.vue'
import Showcase from './components/Showcase.vue'

export default {
  name: 'App',
  components: {
    Navigation,
    Welcome,
    Showcase
  }
}
</script>

<style>
  @import './assets/styles/styles.css';
</style>
