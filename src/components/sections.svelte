<script>
    let {children} = $props()
    import "../global.css";
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
        width: 100%;
        height: 100%;

        margin: 0;
        padding: 0;
    }
    
</style>