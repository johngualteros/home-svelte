<script>
	import Header from './Header.svelte';
	import './styles.css';
</script>

<div class="app">
	<Header />

	<main>
		<slot />
	</main>

	<footer>
		<p>visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to learn SvelteKit. made with john Gualteros</p>
	</footer>
</div>

<style>
	footer{
		text-align: center;
		width: 100%;
		padding: 1rem;
		position: fixed;
		bottom: 0;
	}
	a{
		background-image: linear-gradient(120deg, #32a8f8 0%, #b932f8 50%, #ff2768 100%);
		-webkit-background-clip: text;
		-webkit-text-fill-color: transparent;
	}
</style>
