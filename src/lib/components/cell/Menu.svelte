<script lang="ts">
	let className: string = '';

	export { className };
</script>

<menu class={`header-menu-navbar ${className}`}>
	<ul>
		<li><a href="/">Sustentabilidade</a></li>
		<li><a href="/">Economia</a></li>
		<li><a href="/">Notícias</a></li>
		<li><a href="/">Sobre nós</a></li>
	</ul>
</menu>

<style>
	.header-menu-navbar > ul {
		display: flex;
		align-items: center;
		list-style: none;
		gap: 2rem;

		& li > a {
			font-size: 1.3rem;
			text-decoration: none;
			color: #212121;
			font-weight: 600;
			transition: all 300ms;

			&:hover {
				opacity: 0.6;
			}
		}
	}

	@media (max-width: 720px) {
		.header-menu-navbar {
			display: none !important;
		}
	}
</style>
