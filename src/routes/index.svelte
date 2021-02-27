<script>
	import token from './_token.js';
	import Avatar from '../components/Avatar.svelte';
	import Row from '../components/Row.svelte';
	import Col from '../components/Col.svelte';
	import Separator from '../components/Separator.svelte';
	import Price from '../components/Price.svelte';
	import Button from '../components/Button.svelte';
	import Image from '../components/Image.svelte';
</script>

<style>
	h1 {
		font-weight: bold;
		font-size: 2.5em;
		margin-bottom: 0;
	}
	img {
		width: 100%;
		max-width: 400px;
		margin: 0 0 1em 0;
		border-radius: 10px;
	}
	p {
		margin-top: 15px;
	}
</style>

<svelte:head>
	<title>Debay - {token.name}</title>
</svelte:head>

<Row>
	<Col>
		<Image imageUrl="{token.imageUrl}" />
	</Col>
	<Col>
		<h1>{token.name}</h1>
		<p>{token.description}</p>
		
		<Separator title="owner" />
		<Avatar 
			imageUrl={token.owner.imageUrl} 
			name={token.owner.name}
		/>

		<Separator title="Price" />
		<Price 
			value={token.price.value}
			unit={token.price.unit}
		/>

		<Button>Buy now</Button>
	</Col>
</Row>


