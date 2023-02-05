<script lang="ts">
	let counter = 0;
	let text = '';

	console.log('Hello from page.svelte');

	function increment() {
		counter += 1;
	}
</script>

<h1>Home page</h1>

<p>Counter: {counter}</p>
<button on:click={increment}>Click</button>

<input type="text" bind:value={text} />

<p>Text: {text}</p>

<button on:click={() => (text = '')}>Reset</button>

<p>Some text</p>

<p>Yet another text</p>
