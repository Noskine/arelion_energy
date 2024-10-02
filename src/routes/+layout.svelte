<script>
	import Footer from '$lib/components/Footer.svelte';
	import '../app.css';
</script>

<div class="app">
	<main>
		<slot />
		<Footer />
	</main>
</div>

<style>
</style>
