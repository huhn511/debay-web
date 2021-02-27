<style>
  .col {
		flex: 1;
		width: 100%;
		min-width: 100%;
	}
	
	@media (min-width: 720px) {
		.col {
			margin: 0 15px;
			width: auto;
			min-width: auto;
    }
	}
</style>

<div class="col">
  <slot></slot>
</div>
