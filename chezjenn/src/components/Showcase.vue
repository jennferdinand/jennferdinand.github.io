<template>
  <b-container>
    <h2>Showcase</h2>
    <hr>
    <div class= "div1" v-for="data in foodData" v-bind:key="data">
        <div class="food-card">
            <h4>{{data.name}}</h4>
            <img :src="data.img" width =90%/>
        </div>
    </div>
  </b-container>
</template>

<script>
import foodJson from '../assets/data/food'
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
      return {
        foodData: foodJson
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

h2 {
    text-align: left;
}

h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.food-card {
    width: 95%;
    background: white;
    padding: 0.5em;
    border-style: ridge;
    border-width: 0.1em; 
    border-color: rgba(255, 255, 255, 0.527);
}
</style>
