<script>
    export let name;
    export let icon;
</script>

<div class="skill-pill flex justify-evenly items-center gap-x-2 rounded-lg py-1 px-4">
    {#if icon}
        <img class="w-8" src={icon} alt={name}/>    
    {/if}
    <p class="text-lg">{name}</p>
</div>
