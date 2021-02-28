<script>
	import Nav from '../components/Nav.svelte'
</script>

<main>
	<Nav />
	<slot/>
</main>

<style>
	:global(:root){
		/* CI Colors */
		--color-white: white;
		--color-light: #fbfbfb;
		--color-dark: #041027;
		--color-black: #000817;
		--color-primary: rgba(52, 116, 235);

		/* Element Colors */
		--color-page: var(--color-light);
		--color-layout: var(--color-white);
		--color-text: var(--color-black);
		--color-button: var(--color-primary);

		/* Globals */
		--radius: 10px;
		--box-shadow: 0 0 6px rgba(0,0,0,0.25);
		--border: 2px solid rgba(0,0,0,0.15);
		--content-width: 1200px;

		/* Spacing */
		--space-xxxs: 2px;
		--space-xxs: 4px;
		--space-xs: 8px;
		--space-sm: 12px;
		--space-md: 16px;
		--space-lg: 24px;
		--space-xl: 32px;
		--space-xxl: 40px;
		--space-xxxl: 48px;
	}

	:global(body) {
		background-color: var(--color-page);
		color: var(--color-text);
		transition: background-color 0.3s;
	}

	:global(body.dark-mode) {
		--color-page: var(--color-dark);
		--color-layout: var(--color-black);
		--color-text: var(--color-white);
	}

	:global(*) {
		box-sizing: border-box;
		font-family: Roboto, -apple-system, BlinkMacSystemFont, Segoe UI, Oxygen, Ubuntu, Cantarell, Fira Sans, Droid Sans, Helvetica Neue, sans-serif;
	}
	
	:global(main) {
		top: calc(2 * var(--space-xxxl));
		position: relative;
		width: 100%;
		padding: var(--space-lg);
		box-sizing: border-box;
	}

	:global(h1) {
		font-weight: bold;
		font-size: var(--space-xxxl);
		margin-top: 0;
		margin-bottom: var(--space-sm);
	}

	:global(p) {
		font-size: var(--space-md);
		line-height: 1.5;
		opacity: 0.75;
		margin: 0 0 var(--space-lg);
	}

</style>
