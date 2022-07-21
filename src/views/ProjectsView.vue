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
		<div class="projectFilter" v-if="filteredProjects">
			<select v-model="language">
				<option value="all">All</option>
				<option value="CSS">CSS</option>
				<option value="JAVASCRIPT">Javascript</option>
				<option value="BOOTSTRAP">Bootstrap</option>
				<option value="VUE">Vue</option>
			</select>
		</div>
		<div class="cardholder">
			<Projectcard
				v-for="project of filteredProjects"
				:key="project.id"
				:project="project"
			/>
		</div>
	</section>
</template>
<script>
	import Icons from "@/components/icons.vue";
	import Projectcard from "../components/projectcard.vue";

	export default {
		computed: {
			filteredProjects() {
				return this.projects.filter((project) => {
					let isMatch = true;
					if (this.language !== "all" && project.language !== this.language)
						isMatch = false;
					return isMatch;
				});
			},
		},
		data() {
			return {
				projects: [
					{
						id: "1",
						img: "https://i.postimg.cc/Vk9zYRtg/Screenshot-2022-07-21-095105.jpg",
						title: "ToDoList",
						description: "",
						language: "JAVASCRIPT",
						date: "",
						github: "",
						livelink: "",
					},
					{
						id: "2",
						img: "https://i.postimg.cc/0jJqhdxp/Screenshot-2022-07-21-095132.jpg",
						title: "Car Website",
						description: "",
						language: "JAVASCRIPT",
						date: "",
						github: "",
						livelink: "",
					},
					{
						id: "3",
						img: "https://i.postimg.cc/tg2y642V/Screenshot-2022-07-21-095033.jpg",
						title: "BMI Calculator",
						description: "",
						language: "JAVASCRIPT",
						date: "",
						github: "",
						livelink: "",
					},
					{
						id: "4",
						img: "https://i.postimg.cc/G2fCMS0L/Screenshot-2022-07-21-095048.jpg",
						title: "Weather Converter",
						description: "",
						language: "JAVASCRIPT",
						date: "",
						github: "",
						livelink: "",
					},
					{
						id: "5",
						img: "https://i.postimg.cc/7b8y4GYj/Screenshot-2022-07-21-094939.jpg",
						title: "Restaurant Website",
						description: "",
						language: "BOOTSTRAP",
						date: "",
						github: "",
						livelink: "",
					},
					{
						id: "6",
						img: "https://i.postimg.cc/9M02YHng/Screenshot-2022-07-21-095153.jpg",
						title: "Game Website",
						description: "",
						language: "VUE",
						date: "",
						github: "",
						livelink: "",
					},
					{
						id: "7",
						img: "https://i.postimg.cc/2SNzRJ13/Screenshot-2022-07-21-094959.jpg",
						title: "Second Portfolio",
						description: "",
						language: "CSS",
						date: "",
						github: "",
						livelink: "",
					},
					{
						id: "8",
						img: "https://i.postimg.cc/43Jsn9bg/Screenshot-2022-07-21-095015.jpg",
						title: "Calculator",
						description: "",
						language: "JAVASCRIPT",
						date: "",
						github: "",
						livelink: "",
					},
				],
				language: "all",
			};
		},
		components: { Projectcard, Icons, Icons, Icons, Icons, Projectcard },
	};
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
		font-family: Rocket;
		text-shadow: 3px 3px black;
		letter-spacing: 1px;
		font-size: 30px;
	}
	.heading {
		color: #67b3e4;
		font-family: SpaceQuest;
		letter-spacing: 3px;
		text-shadow: 2px 2px black;
	}

	/*  */

	.cardholder {
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		justify-content: center;
		align-items: center;
		gap: 45px;
	}
	.projectFilter {
		display: flex;
		flex-direction: row;
		flex-wrap: nowrap;
		justify-content: center;
		align-content: center;
		margin-bottom: 5%;
	}
	select {
		width: 190px;
		height: 50px;
		filter: drop-shadow(4px 4px 4px grey);
	}
	/*  */
</style>
