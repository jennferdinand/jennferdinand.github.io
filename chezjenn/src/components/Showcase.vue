<template>
	<b-container>
		<h2 id="showCase">Showcase</h2>
		<hr />
		<h3 id="deserts">Deserts</h3>
		<span v-for="data in foodData" v-bind:key="data">
			<div class="div1" v-if="data.category =='desert'">
				<div class="food-card">
					<h4>{{data.name}}</h4>
					<img :src="data.img" width="90%" />
				</div>
			</div>
		</span>
		<h3 id="mains">Mains</h3>
		<span v-for="data in foodData" v-bind:key="data">
			<div class="div1" v-if="data.category =='main'">
				<div class="food-card">
					<h4>{{data.name}}</h4>
					<img :src="data.img" width="90%" />
				</div>
			</div>
		</span>
	</b-container>
</template>

<script>
import foodJson from "../assets/data/food";
export default {
	name: "Showcase",
	props: {
		msg: String
	},
	data() {
		return {
			foodData: foodJson
		};
	}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h2 {
	text-align: left;
}

h3 {
	text-align: left;
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
	border-style: groove;
	border-width: 0.05em;
	border-color: rgba(255, 255, 255, 0.527);
}
</style>
