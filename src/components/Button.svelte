<script>
	export let callback
</script>

<style>
  button {
		background-color: var(--color-primary);
		outline: none;
		border-radius: 100px;
		border: var(--border);
		padding: var(--space-md);
		font-size: var(--space-md);
		color: var(--color-white);
		display: block;
		width: 100%;
		font-weight: bold;
		cursor: pointer;
	}
</style>

<button on:click={callback}>
	<slot/>
</button>
