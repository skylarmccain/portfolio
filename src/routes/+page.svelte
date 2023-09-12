<script>
	import { base } from '$app/paths';
	import FaLinkedin from "svelte-icons/fa/FaLinkedin.svelte";
	import FaGithub from "svelte-icons/fa/FaGithub.svelte";
	import MemojiImage from "../static/images/Memoji.png";
	import { Hamburger } from "svelte-hamburgers";
    import Sidebar from "../lib/components/Sidebar.svelte";

    let open = false;
</script>


<svelte:head>
	<title>Skylar McCain - Main page</title>
</svelte:head>
<nav class="flex flex-row-reverse bg-base-200">
	<Hamburger bind:open />
</nav>
<Sidebar bind:open />
<div class="snap-y snap-mandatory min-h-screen bg-base-200">
	<div class="snap-center snap-always hero">
		<div class="hero-content flex-col lg:flex-row">
			<img src={MemojiImage} class="px-12"/>
			<div>
				<h1 class="text-5xl font-bold">Hi, I'm Skylar! 👋</h1>
				<p class="py-4 text-2xl font-medium">
					I am a designer and front-end developer.
				</p>
				<p class="text-xl">
					I am passionate about creating human-centered products that harmonize the user experience with technology. 
					With a background in software development and UX design, I aspire to leverage my skills to build innovative products that offer impactful solutions and exceptional user experiences. 
				</p>
				<div class="flex flex-row gap-5 pt-4">
					<a href="https://github.com/skylarmccain" target="_blank" class="link">
						<div class="icon">
							<FaGithub />
						</div>
					</a>
					<a href="https://www.linkedin.com/in/skylarmccain/" target="_blank" class="link">
						<div class="icon">
							<FaLinkedin />
						</div>
					</a>
				</div>
			</div>
		</div>
	</div>
	<!-- <section class="bg-black snap-center min-h-screen snap-always">
		<h1 class="text-5xl font-bold py-20">TEST</h1>
	</section> -->
</div>

<style>

	.icon {
		cursor: pointer;
		transition: color 0.2s ease-in-out;
		width: 40px;
	}
</style>
