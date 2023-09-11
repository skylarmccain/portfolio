<script>
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
<div class="snap-y snap-mandatory min-h-screen bg-base-200">
	<nav class="flex flex-row-reverse">
		<Hamburger bind:open />
	</nav>
	<Sidebar bind:open />
	<div class="snap-center snap-always hero">
		<div class="hero-content flex-col lg:flex-row">
			<img src={MemojiImage} class="px-12"/>
			<div>
				<h1 class="text-5xl font-bold">Hi, I'm Skylar! 👋</h1>
				<p class="py-4 text-lg">
					I am a software developer, passionate about building
					products that are centered around the user experience.
				</p>
				<div class="flex flex-row gap-5">
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
