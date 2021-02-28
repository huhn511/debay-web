<script>
	import nft from './_nft.js'

	import Avatar from '../components/Avatar.svelte'
	import Row from '../components/Row.svelte'
	import Container from '../components/Container.svelte'
	import Col from '../components/Col.svelte'
	import Separator from '../components/Separator.svelte'
	import Price from '../components/Price.svelte'
	import Button from '../components/Button.svelte'
	import Image from '../components/Image.svelte'

	const buyNFT = () => {
    console.log('This will soon open your wallet.')
  }
</script>

<svelte:head>
	<title>Debay - {nft.name}</title>
</svelte:head>
<Container>
	<Row>
		<Col>
			<Image imageUrl="{nft.imageUrl}" />
		</Col>
		<Col>
			<h1>{nft.name}</h1>
			<p>{nft.description}</p>
			
			<Separator title='owner' />
			<Avatar
				imageUrl={nft.owner.imageUrl} 
				name={nft.owner.name}
			/>

			<Separator title='Price' />
			<Price 
				value={nft.price.value}
				unit={nft.price.unit}
			/>

			<Button callback={buyNFT}>Buy now</Button>
		</Col>
	</Row>
</Container>

