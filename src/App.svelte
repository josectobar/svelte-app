<script lang="ts">
	let count = 0
	
	function increment() {
		count +=1
	}
</script>

<h1>Animated Buttons</h1>
<p>{count}</p>
<button on:click={increment}>
	Click here!
</button>

<button on:click={() => count = 0}>
	Reset
</button>