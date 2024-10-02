<script lang="ts">
	let className: string = '';

	let isDark: boolean;

	export { className, isDark };
</script>

<menu class={`header-menu-navbar ${className}`}>
	<ul>
		<li><a class={isDark ? 'dark' : ''} href="/">Sustentabilidade</a></li>
		<li><a class={isDark ? 'dark' : ''} href="/">Economia</a></li>
		<li><a class={isDark ? 'dark' : ''} href="/">Notícias</a></li>
		<li><a class={isDark ? 'dark' : ''} href="/">Sobre nós</a></li>
	</ul>
</menu>

<style>
	.dark {
		color: #212121 !important;
	}

	.header-menu-navbar > ul {
		display: flex;
		align-items: center;
		list-style: none;
		gap: 2rem;

		& li > a {
			font-size: 1.3rem;
			text-decoration: none;
			color: #f1f1f1;
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
