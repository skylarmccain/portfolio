<script>
    /** @type {import('./$types').PageData} */
    export let data;
    import ProjectCard from "../../lib/components/ProjectCard.svelte";
    import { Hamburger } from "svelte-hamburgers";
    import Sidebar from "../../lib/components/Sidebar.svelte";

    let open = false;
</script>

<svelte:head>
    <title>Skylar McCain - Projects page</title>
</svelte:head>
<div class="min-h-screen bg-base-200">
<nav class="flex flex-row-reverse bg-base-200">
	<Hamburger bind:open />
</nav>
<Sidebar bind:open />
<div class="snap-y snap-mandatory scroll-auto">
    <div class="flex flex-wrap justify-between mt-10 mx-10 gap-6">
        <!-- Project Cards List -->
       <ProjectCard
            Title="3D Interactive Procedural Terrain Interface"
            Description="Created a desktop application in Processing that generated a 3D terrain map from an imported file or user designed terrain using UI elements
            User could personalize polygon count, terrain size, terrain height, and color blending
            Implemented camera that allowed user to explore map by modifying camera angle with mouse interactions
            "
        />
        <ProjectCard
            Title="Gesture Recognition Application"
            SkillsRequired="python, object-oriented programming, data structures, algorithm design, GUI development, Git"
            Description="Worked with team to implement $1 and $N recognition algorithms (python)
            Coded preprocessing of gesture input that transformed coordinates to standardized objects to compare with templates
            Devised and executed an offline testing algorithm
            Generated speed and accuracy improvements to recognition algorithm based on offline test results
            "/>
        <ProjectCard
        Title="File Input Program and GUI Application"
        SkillsRequired="Linux OS/Filesystem, file I/O, C++ "
        Description="Created program that read text files via POSIX calls and output text to GUI application
        Tested for data leaks in program using C++ Memory Validator
        Identified program errors, such as unreadable file input or read permissions, and created error catches for the issues
        " />
        <ProjectCard
        Title="Online Client Portal"
        SkillsRequired="React, Web Development, Agile, semantic ui, CSS, MongoDB, Git, Figma"
        Description="Worked with Gainesville law firm to develop a client-communication portal
        Styled all components, programmed page layouts
        Constructed front-end code for calendar page with individualized user content to display appointments, events, and deadlines
        "/>
        <ProjectCard
        Title="GatorPool Web App"
        SkillsRequired="React, CSS, UX Design Principles"
        Description="Designed and prototyped virtual platform for UF student carpool/transportation as HCI class assignment
        Coded style and simple front-end functionality in React
        Focused on design process: conducted focus groups, usability tests, user research, iterative prototyping"
         />
         <ProjectCard
         Title="Explaore NASA Images Application"
         SkillsRequired="Unreal Engine, UMG, REST APIs, JSON, C++"
         Description="Created a UI that displayed NASA Images populated from NASA API at runtime. Incorporated Common UI plugin to project architecture to enable cross-platform scaling 
         Optimized rendering through asynchronous populating of UI components by staggering HTTP request for image data from the API.  
         "
         />
    </div>
</div>
</div>
