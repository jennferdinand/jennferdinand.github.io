<template>
	<b-navbar toggleable="lg" type="light">
		<b-navbar-brand id="brand" href="#">chezjenn</b-navbar-brand>
		<b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
		<b-collapse id="nav-collapse" is-nav>
			<b-navbar-nav>
				<b-nav-item href="https://www.instagram.com/chezjenn" target="_blank">
					<i class="fab fa-instagram"></i>
				</b-nav-item>
				<b-nav-item href="#deserts">Deserts</b-nav-item>
				<b-nav-item href="#mains">Mains</b-nav-item>
			</b-navbar-nav>
		</b-collapse>
	</b-navbar>
</template>

<script>
export default {
	name: "Navigation",
	props: {
		msg: String
	},
	methods: {
		scrollToTop() {
			document.documentElement.scrollTop = 0;
			history.pushState("", document.title, window.location.pathname);
		}
	},
	mounted: function() {
		document.getElementById("brand").onclick = this.scrollToTop;
	}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.navbar {
    position: fixed;
    top: 0;
    width: 100%;
  background: rgba(254, 250, 255, 0.513);
}

</style>
