<script>
	import Menu from './cell/Menu.svelte';
	import src from '$lib/images/logoAlternativo.png';
</script>

<section class="content-footer-page">
	<hr />
	<footer>
		<img {src} class="logotype-footer" alt="logotype arelion sol energy" />
		<Menu isDark={false} />
	</footer>
</section>

<style>
	.content-footer-page {
		padding-inline: 5%;
    color: #f1f1f195;
	}

	footer {
		display: flex;
		align-items: center;
		justify-content: space-between;
		margin-block: 20px;
	}

	.logotype-footer {
		width: 100px;
	}
</style>
