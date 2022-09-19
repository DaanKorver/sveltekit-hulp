<script>
	//Dit zijn props (properties) van de component
	//Deze kan je gebruiken om een component uniek te maken
	//Je kan props gebruiken voor content, maar denk ook aan links (href), image paths of booleans (true / false)
	export let title;
	export let text;
</script>

<section>
	<h3>{title}</h3>
	<p>{text}</p>
</section>

<style>
	section {
		width: 25rem;
		height: auto;
		padding: 1em;
		background-color: blue;
		margin-bottom: 1rem;
	}
</style>
