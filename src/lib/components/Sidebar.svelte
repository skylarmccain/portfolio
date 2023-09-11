<script>
	export let open = false
</script>

<aside class="absolute bg-teal-900 justify-end flex" class:open>
	<nav class="p-12 text-base-100 font-semibold text-5xl">
		<a class="block hover:text-base-200 py-4 text-end" href="/">About</a>
		<a class="block hover:text-base-200 py-4 text-end" href="projects">Projects</a>
	</nav>
</aside>

<style>
	aside {
		width: 0px;
		transition: right 0.3s ease-in-out;
		z-index: 0;
	}
	
	.open {
		right: 0;
		width: 100%;
		height: 100%;
		z-index: 10;
	}
</style>