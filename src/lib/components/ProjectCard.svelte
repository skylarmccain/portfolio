
<script>
    export let Title;
    export let Description;
    export let SkillsRequired;
</script>
<div class="p-4 max-w-sm border-4 bg-teal-900 bg-opacity-20 border-teal-900 rounded-2xl">
    <div class="text-xl font-medium">
        {Title}
    </div>
    <div >
        {#if SkillsRequired}
        <p class="font-medium">Skills Required: {SkillsRequired}</p>
        {/if}
        <p class="py-3">{Description}</p>
    </div>
</div>