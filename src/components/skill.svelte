<script>
    export let name;
    export let icon;
</script>

<div class="flex justify-evenly items-center gap-x-2 bg-indigo-400 rounded-lg py-1 px-4">
    {#if icon}
        <img class="w-8" src={icon} alt={name}/>    
    {/if}
    <p class="text-lg">{name}</p>
</div>
