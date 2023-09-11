<script>
    /** @type {import('./$types').LayoutData} */
    import "../app.css";
    export let data;
    export const prerender = true;
    import { Hamburger } from "svelte-hamburgers";
    import Sidebar from "../lib/components/Sidebar.svelte";

    let open = false;
</script>


    <slot/>


