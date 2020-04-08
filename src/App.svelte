<script>
	import Git from './github.svelte';
	import Git2 from './github.svelte';
</script>

<main>
<p>Without Single value</p>
	<Git />
	<hr/>
	<p>SIngle value</p>
		<Git2 single="1"/> 
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>