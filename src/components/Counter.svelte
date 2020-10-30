<script>
    let count = 0;
</script>

<style>
    div {
        background: lightblue;
        width: 300px;
        margin: 0 auto;
        border-radius: 20px;
    }
    button {
        padding: 2px;
    }
</style>

<div>
    <h1>The count is: {count}</h1>
    <button
        on:click={() => {
            count += 1;
        }}>+</button>
</div>
