<template>
	<section id="projects">
		<h2 class="heading">- some of my work -</h2>
		<h1 class="heading-">PROJECTS</h1>
		<div class="projects-section">
			<div class="projectdesc">
				<main class="container">
					<div class="bckgd-globe1"></div>
					<div class="glass-card">
						<div class="card-content">
							<div class="blurred"></div>
							<span>03</span>
							<h3>Card Three</h3>
							<p>
								Lorem ipsum dolor sit amet consectetur, adipisicing elit.
								Eveniet sunt, omnis hic animi officiis iste, veniam asperiores
								fugit recusandae illum sint.
							</p>
							<button>Read more</button>
						</div>
					</div>
				</main>
			</div>
			<div class="iphone">
				<img
					class="png1"
					src="https://i.postimg.cc/WbYX5Znz/pngwing-com-1.png"
					alt=""
				/>
			</div>

			<div class="laptop">
				<img
					class="png2"
					src="https://i.postimg.cc/K8dQ2yCy/pngwing-com.png"
					alt=""
				/>
			</div>
		</div>
	</section>
</template>
<script>
	export default {};
</script>
<style scoped>
	#projects {
		max-height: 100vh;
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
		margin-bottom: 20%;
		margin-top: -2%;
		display: flex;
		flex-wrap: nowrap;
		flex-direction: row;
		justify-content: center;
		align-items: center;
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
		justify-content: start;
		align-items: flex-start;
		margin-top: 10%;
		height: 500px;
		width: 300px;
	}
	.laptop {
		display: flex;
		flex-direction: row;
		flex-wrap: nowrap;
		justify-content: end;
		align-items: end;
		width: 600px;
		height: 400px;
		margin-top: 17%;
	}
	.png1 {
		height: 500px;
		width: 300px;
	}
	.png2 {
		width: 600px;
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

	.bckgd-globe1 {
		position: absolute;
		width: 200px;
		height: 200px;
		background-image: linear-gradient(rgb(0, 127, 185), rgb(140, 103, 209));
		border-radius: 500px;
		margin-top: 20%;
		margin-left: 2%;
	}

	.glass-card {
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		justify-content: start;
		align-items: flex-start;
		backdrop-filter: blur(10px);
		max-width: 300px;
		height: 500px;
		margin-top: 30%;
	}

	.blurred {
		position: absolute;
		left: 0;
		top: 0;
		width: 100%;
		height: 100%;
		background: rgba(255, 255, 255, 0.15);
		border-radius: 12px;
		box-shadow: 15px 15px 15px 0 rgba(0, 0, 0, 0.3);
	}

	.card-content {
		padding: 5rem 2rem;
		position: relative;
		left: 0;
		top: 0;
		width: 100%;
		height: 100%;
		border-top: 2px solid rgba(255, 255, 255, 0.4);
		border-left: 2px solid rgba(255, 255, 255, 0.4);
		border-right: 3px solid rgba(255, 255, 255, 0.32);
		border-bottom: 3px solid rgba(255, 255, 255, 0.32);
		border-radius: 15px;
		background: linear-gradient(
			135deg,
			transparent 0%,
			transparent 8%,
			rgba(255, 255, 255, 0.03) 30%,
			rgba(255, 255, 255, 0.03) 60%,
			rgba(255, 255, 255, 0) 68%
		);
	}

	.glass-card span {
		position: absolute;
		left: 50%;
		top: 5%;
		transform: translateX(-50%);
		font-size: 6.25em;
		color: rgba(255, 255, 255, 0.1);
		font-weight: 700;
	}

	.glass-card h3 {
		font-size: 2.2em;
		color: rgba(255, 255, 255, 0.85);
	}

	.glass-card p {
		margin: 1em 0;
		color: #fff;
		line-height: 1.4;
	}

	.glass-card button {
		border: 0 none;
		font-size: 1.125em;
		color: #444;
		padding: 0.6em 1.1em 0.7em;
		border-radius: 100px;
	}
</style>
