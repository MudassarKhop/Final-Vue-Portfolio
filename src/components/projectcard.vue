<template>
	<div class="card">
		<div id="img">
			<img v-bind:src="project.img" alt="" />
		</div>
		<div id="h1">
			<h1>{{ project.title }}</h1>
		</div>

		<button>
			<a href="project.githhub" target="blank"> </a>
			GITHUB
		</button>
		<button>
			<a href="project.livelink" target="blank"></a>
			LIVE LINK
		</button>
	</div>
</template>
<script>
	export default {
		props: ["project"],
	};
</script>
<style scoped>
	#img {
		position: relative;
		bottom: 12%;
	}
	img {
		position: relative;
		height: 240px;
		width: 290px;
		border-top-left-radius: 8%;
		border-top-right-radius: 8%;
	}
	#h1 {
		font-size: small;
	}
	.card {
		background: #191c29;
		width: 290px;
		height: 460px;
		padding: 3px;
		border-radius: 6px;
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		justify-content: center;
		align-items: center;
		text-align: center;
		font-size: 1.5em;
		color: white;
		border-top-left-radius: 15%;
		border-top-right-radius: 15%;
		animation: floating 4s ease-in-out infinite;
		filter: drop-shadow(4px 4px 4px grey);
	}
	button {
		display: none;
		width: 80px;
		height: 30px;
	}
	.card:hover {
		filter: none;
		box-shadow: 0 0px 7px 9px rgba(58, 39, 96, 0.6);
		transition: box-shadow 0.5s ease-in-out;
		transition: filter 0.5s ease-in-out;
	}
	.card:hover button {
		display: block;
		color: black;
	}
	@keyframes floating {
		0% {
			transform: translateY(0);
		}
		50% {
			transform: translateY(-16px);
		}
		100% {
			transform: translateY(0);
		}
	}
</style>
