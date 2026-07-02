<script>
    let isActive = $state(false);
</script>

<button onclick={() => isActive = !isActive}>
    <div class:active={isActive}>
        <h1>Hello</h1>
    </div>
</button>

<style>

    div {
        width: 500px;
        height: 250px;

        transition: all 0.5s ease-out;
    }

    div:hover {
        scale: 1.1;
    }

    .active {
        background-color: red;
    }
</style>
