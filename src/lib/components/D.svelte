<script>
    let w = 0;
</script>
<svelte:window bind:innerWidth={w}></svelte:window>
{#if w > 700}
<span>▪</span>
{/if}
<style>
    span {
        padding:20px;
    }
</style>