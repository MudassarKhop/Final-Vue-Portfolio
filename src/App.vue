<template>
	<router-view />
</template>
<script></script>
<style>
	* {
		padding: 0;
		margin: 0;
		box-sizing: border-box;
	}
	#app {
		font-family: Avenir, Helvetica, Arial, sans-serif;

		color: white;
	}

	nav {
		padding: 30px;
	}

	nav a {
		font-weight: bold;
		color: #2c3e50;
	}

	nav a.router-link-exact-active {
		color: #42b983;
	}
</style>
