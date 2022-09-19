<script>
	import Card from '../lib/components/Card.svelte';

	//Deze data zou bijvoorbeeld uit een database kunnen komen (Prismic.io)
	const kaarten = [
		{
			title: 'Eerste kaart',
			text: 'Tweede'
		},
		{
			title: 'Tweede kaart',
			text: 'Fancy'
		},
		{
			title: 'Drieeeee',
			text: 'Loops zijn awesome'
		}
	];
</script>

<h1>Components</h1>
<!-- Je kan components nu hergebruiken met verschillende content -->
<Card title={'Kaart nummer een!'} text={'Hier kan tekst komen'} />
<Card title={'Twee!'} text={'Hier kan een andere tekst'} />
<Card title={'Nummer drie!'} text={'Tekst van de 3de'} />
<Card title={'Nummertje 4'} text={'Laatste kaartje'} />

<h2>Met een loop</h2>
<!-- Je kan ook een loop gebruiken (dit kan handig zijn als je data krijg van een) -->
{#each kaarten as kaart}
	<Card title={kaart.title} text={kaart.text} />
{/each}
