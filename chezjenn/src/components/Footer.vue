<template>
	<b-container>
		<footer class="FooterClass" id="footerComponent">
			<p></p>
			<div class="links">

			</div>
		</footer>
	</b-container>
</template>

<script>
export default {
	name: "Footer",
	methods: {
	},
	mounted: function() {
		var year = new Date().getFullYear();
		document.querySelector("footer p").innerHTML =
			"Copyright &#169 " + year + " Jennifer Ferdinand";
	}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
