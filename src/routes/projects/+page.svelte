<script>
    /** @type {import('./$types').PageData} */
    export let data;
    import { Hamburger } from "svelte-hamburgers";
    import Sidebar from "../../lib/components/Sidebar.svelte";
    import ProjectCard from "../../lib/components/ProjectCard.svelte";

    let open = false;
</script>

<svelte:head>
    <title>Skylar McCain - Projects page</title>
</svelte:head>
<div class="snap-y snap-mandatory scroll-auto min-h-screen bg-base-200">
    <nav class="flex flex-row-reverse">
        <Hamburger bind:open />
    </nav>
    <Sidebar bind:open />
    <div class="flex flex-wrap justify-between mt-10 mx-10">
        <!-- Project Cards List -->
       <ProjectCard
            Title="3D Interactive Procedural Terrain Interface"
            Description="Created a desktop application in Processing that generated a 3D terrain map from an imported file or user designed terrain using UI elements
            User could personalize polygon count, terrain size, terrain height, and color blending
            Implemented camera that allowed user to explore map by modifying camera angle with mouse interactions
            "
        />
    </div>
</div>
