<script>
	import Logo from './cell/Logo.svelte';
	import Menu from './cell/Menu.svelte';
	import { CirclePlus, CircleChevronLeft } from 'lucide-svelte';
</script>

<header class="app-header-navbar">
	<Logo />
	<Menu />
	<button class="header-navbar-contact-us">
		Orçamento
		<CirclePlus size={16} />
	</button>
	<button class="header-mobile-button-navbar">
		<CircleChevronLeft size={19} />
	</button>
</header>

<style>
	.app-header-navbar {
		display: flex;
		justify-content: space-between;
		align-items: center;
		padding: 10px 5%;

		& .header-mobile-button-navbar {
			display: none;
			background-color: transparent;
			border: none;
			align-items: center;
			justify-content: center;
			color: var(--color);
			cursor: pointer;
		}

		& .header-navbar-contact-us {
			display: flex;
			align-items: center;
			justify-content: center;
			gap: 5px;
			background-color: transparent;
			color: var(--color);
			border: 1px solid var(--color);
			padding: 5px 20px;
			border-radius: 8px;
			font-size: 1.2rem;
			font-weight: 600;
			transition: all 300ms ease-in;
			backdrop-filter: blur(1px);
			-webkit-backdrop-filter: blur(1px);
			box-shadow: var(--shadow);
			cursor: pointer;

			& svg {
				transition: all 300ms ease-in;
			}

			&:hover {
				opacity: 0.6;
				& svg {
					transform: rotate(135deg);
				}
			}
		}
	}

	@media (max-width: 720px) {
		.header-navbar-contact-us {
			display: none !important;
		}
		.header-mobile-button-navbar {
			display: flex !important;
		}
	}
</style>
