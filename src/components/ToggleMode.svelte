<script>
	import Moon from './icons/Moon.svelte'

  function toggle() {
    window.document.body.classList.toggle('dark-mode')
  }
</script>

<style>
  button {
		background-color: var(--color-primary);
		outline: none;
		border-radius: 100px;
		border: var(--border);
		width: var(--space-xxxl);
		height: var(--space-xxxl);
		font-size: 1em;
		display: flex;
		justify-content: center;
		align-items: center;
		color: var(--color-white);
		cursor: pointer;
	}
</style>

<button on:click={toggle}>
	<Moon />
</button>
