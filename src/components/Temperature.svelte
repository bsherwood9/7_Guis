<script>
    let f = 0;
    let c = ((f - 32) * (5 / 9)).toFixed(2);

    function inputHandler(type) {
        if (type === "f") {
            c = ((f - 32) * (5 / 9)).toFixed(2);
        }
        if (type === "c") {
            f = (c * (9 / 5) + 32).toFixed(2);
        }
    }
</script>

<style>
    div {
        background: lightgreen;
        width: 550px;
        margin: 20px auto;
        border-radius: 20px;
        display: flex;
        justify-content: center;
    }
    input {
        width: 100px;
    }
    label {
        font-size: 28px;
    }
</style>

<div>
    <label for="fahr"> Fahrenheit</label>
    <input
        type="number"
        id="fahr"
        bind:value={f}
        on:input={() => {
            inputHandler('f');
        }} />

    <label for="cels"> Celsius</label>

    <input
        type="number"
        id="cels"
        bind:value={c}
        on:input={() => {
            inputHandler('c');
        }} />
</div>
