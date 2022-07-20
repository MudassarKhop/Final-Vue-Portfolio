<template>
	<section id="projects">
		<h2 class="heading">- some of my work -</h2>
		<h1 class="heading-">PROJECTS</h1>
		<div class="projects-section">
			<div class="iphone">
				<img
					class="png1"
					src="https://i.postimg.cc/SNyYbngh/Screenshot-2022-07-20-133024.png"
					alt=""
				/>
			</div>
			<div class="laptop">
				<img
					src="https://i.postimg.cc/vHFKXs8k/Screenshot-2022-07-20-133058-1.png"
					alt=""
					class="png2"
				/>
			</div>
		</div>
		<div class="cardholder">
			<div class="card">Magic Card</div>
			<div class="card">Magic Card</div>
			<div class="card">Magic Card</div>
			<div class="card">Magic Card</div>
			<div class="card">Magic Card</div>
		</div>
	</section>
</template>
<script>
	export default {};
</script>
<style scoped>
	#projects {
		min-height: 100vh;
		padding: 50px;
		background: black
			linear-gradient(
				255.21deg,
				rgba(58, 39, 96, 0.6) 12.4%,
				rgba(25, 16, 41, 0.6) 33.1%,
				rgba(26, 23, 47, 0.6) 57.29%,
				rgba(32, 43, 65, 0.6) 77.17%,
				rgba(35, 99, 118, 0.6) 99.74%
			);
	}
	.projects-section {
		display: flex;
		flex-wrap: nowrap;
		flex-direction: row;
		justify-content: center;
		margin-left: 10%;
	}
	.projectdesc {
		display: flex;
		flex-direction: column;
		flex-wrap: nowrap;
		justify-content: center;
		align-items: center;
	}
	.iphone {
		display: flex;
		flex-direction: row;
		flex-wrap: nowrap;
		justify-content: center;
		align-items: center;
		margin-top: 5%;
	}
	.laptop {
		display: flex;
		flex-direction: row;
		flex-wrap: nowrap;
		justify-content: start;
		align-content: flex-start;
		margin-top: 10%;
	}

	.png1 {
		height: 500px;
		width: 250px;
	}
	.png2 {
		width: 780px;
		height: 400px;
	}

	.heading- {
		color: white;
	}
	.heading {
		background: #67b3e4; /* fallback for old browsers */
		background: -webkit-linear-gradient(
			to right,
			#67b3e4,
			#c292de
		); /* Chrome 10-25, Safari 5.1-6 */
		background: linear-gradient(
			to right,
			#67b3e4,
			#c292de
		); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
		-webkit-background-clip: text;
		background-clip: text;
		color: transparent;
		font-family: SpaceQuest;
		letter-spacing: 3px;
	}

	/*  */

	.cardholder {
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		justify-content: center;
		align-items: center;
		gap: 30px;
	}
	.card {
		background: #191c29;
		width: 250px;
		height: 400px;
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
	}
	.card:hover {
		box-shadow: 0 0px 7px 9px rgba(58, 39, 96, 0.6);
		transition: box-shadow 0.3s ease-in-out;
	}
	/*  */
</style>
