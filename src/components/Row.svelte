<style>
  .row {
		display: flex;
    flex-wrap: wrap;
	}
  @media (min-width: 720px) {
    .row {
      justify-content: space-between;
      margin: 0 -15px;
      flex-wrap: nowrap;
    }
	}
</style>

<div class="row">
  <slot></slot>
</div>
