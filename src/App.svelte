<script>
	let name = "7 GUI's";
	import Counter from "./components/Counter.svelte";
	import Temperature from "./components/Temperature.svelte";
</script>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>

<main>
	<h1>Hello {name}!</h1>
	<Counter />
	<Temperature />
</main>
