<template>
  <div id="app">
    <Welcome />
    <Showcase />
  </div>
</template>

<script>
import Welcome from './components/Welcome.vue'
import Showcase from './components/Showcase.vue'

export default {
  name: 'App',
  components: {
    Welcome,
    Showcase
  }
}
</script>

<style>
  @import './assets/styles/styles.css';
</style>
