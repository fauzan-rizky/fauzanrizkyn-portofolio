<script>
    let {children} = $props()
</script>
<div class="sections">
    {#if children}
        {@render children()}
    {/if}
</div>

<style>
    .sections {
        display: flex;
        align-items: center;
        justify-content: center;

        background-color: black;
        color: rgb(255, 230, 0);
        width: 100vw;
        height: 100vh;

        margin: 0;
        padding: 0;
    }
    
</style>