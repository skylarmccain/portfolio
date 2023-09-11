
<script>
    export let Title;
    export let Description;
</script>
<div class="collapse p-4 max-w-sm border-4 bg-teal-900 bg-opacity-20 border-teal-900">
    <input type="checkbox" />
    <div class="collapse-title text-xl font-medium">
        {Title}
    </div>
    <div class="collapse-content">
        <p>{Description}</p>
    </div>
</div>