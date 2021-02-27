<script>
  export let value
  export let unit
</script>

<style>
  .price {
		display: flex;
		align-items: flex-end;
		margin-bottom: 20px;
	}

	h3 {
		font-size: 2em;
		font-weight: bold;
		margin: 0 5px 0 0;
	}

	span {
		margin-bottom: 2px;
	}
</style>

<div class="price">
	<h3>{value}</h3>
	<span>{unit}</span>
</div>
