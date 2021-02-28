<style>
  .container {
		max-width: var(--content-width);
    margin: 0 auto;
	}
  @media (min-width: 720px) {
    .container {
      width: 100%;
    }
	}
</style>

<div class='container'>
	<slot/>
</div>
