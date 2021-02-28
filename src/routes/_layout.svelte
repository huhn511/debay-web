<script>
	import Nav from '../components/Nav.svelte'
</script>

<style>
	:global(:root){
		--color-white: white;
		--color-light: #efefef;
		--color-dark: #2e2e2e;
		--color-black: #181818;
		--color-primary: rgba(52, 116, 235);
		--color-page: var(--color-light);
		--color-button: var(--color-primary);
		--color-text: var(--color-black);
	}

	:global(*) {
		box-sizing: border-box;
	}
	:global(body) {
		background-color: var(--color-page);
	}
	
	:global(main) {
		top: 90px;
		position: relative;
		max-width: 56em;
		padding: 2em;
		margin: 0 auto;
		box-sizing: border-box;
	}

	:global(h1) {
		font-weight: bold;
		font-size: 2.5em;
	}

	:global(p) {
		font-size: 1em;
	}

	:global(body) {
		background-color: var(--color-white);
		color: var(--color-black);
		transition: background-color 0.3s
	}
	:global(body.dark-mode) {
		background-color: var(--color-black);
		color: var(--color-white);
	}
</style>

<main>
	<Nav />
	
	<slot/>
</main>