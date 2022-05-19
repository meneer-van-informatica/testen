<script>
	export let name;
    let count=0;
</script>

<main>
	<h1>Hello {name}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
</main>

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

<button on:click={()=>count++}>
        Increment
</button>
<button on:click={()=>count--}>
        Decrement
</button>
<button on:click={()=>count=0}>
        Reset
</button>

<h2>
        {count}
</h2>