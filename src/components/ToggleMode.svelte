<script>
	import Moon from './icons/Moon.svelte'

  function toggle() {
    window.document.body.classList.toggle('dark-mode')
  }
</script>

<style>
  button {
		background-color: rgba(52, 116, 235);
		outline: none;
		border-radius: 100px;
		border: 2px solid rgba(0,0,0,.1);
		width: 50px;
		height: 50px;
		font-size: 1em;
		display: flex;
		justify-content: center;
		align-items: center;
		color: white;
		cursor: pointer;
	}
</style>

<button on:click={toggle}>
	<Moon />
</button>
