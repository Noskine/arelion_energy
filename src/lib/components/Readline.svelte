<script>
	import Header from './Header.svelte';
	import src from '../images/Placa-Solar-Grupower-2.jpg';
	import { Link } from 'lucide-svelte';
</script>

<section class="readline-home-page" style={`background-image: url(${src})`}>
	<Header />
	<section class="content-readline-text-box">
		<h1 class="text-readline">Economize hoje e começe seu futuro com Arelion Sol Energy</h1>
		<hr class="text-readline" />
		<p class="text-readline">
			Trasforme sua residência/empresa em uma fonte de energia limpa e renovável. Solicite um
			orçamento personalizdo agora mesmo.
		</p>
		<section class="buttons-content-readline">
			<button> Orçamento personalizado </button>
			<button class="budget">
				Notícias
				<Link size={14} />
			</button>
		</section>
	</section>
</section>

<style>
	.text-readline {
		text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.851);
	}

	.readline-home-page {
		position: relative;
		width: 100%;
		height: 100vh;
		background-size: cover;
		z-index: 1;
		overflow: hidden;
		text-shadow: var(--shadow) !important;

		& h1 {
			color: #fff;
			line-height: 50px;
		}

		& hr {
			margin-block: 20px 10px;
		}

		& .buttons-content-readline {
			display: flex;
			align-items: center;
			gap: 10px;
			margin-top: 10px;

			& :nth-child(2) {
				border: 1px solid var(--color);
				background-color: transparent;
				color: var(--color);
				font-weight: 400;
				backdrop-filter: blur(1px);
				-webkit-backdrop-filter: blur(1px);

				&:hover {
					backdrop-filter: blur(1px);
					-webkit-backdrop-filter: blur(1px);
				}
			}

			& > button {
				font-weight: 600;
				display: flex;
				align-items: center;
				justify-content: center;
				gap: 5px;
				width: 50%;
				background-color: #fff;
				color: var(--background);
				border: none;
				border-radius: 5px;
				padding: 5px 15px;
				box-shadow: var(--shadow);
				transition: all 300ms;
				font-size: 1.4rem;
				cursor: pointer;

				&:hover {
					opacity: 0.6;
				}
			}
		}

		&::after {
			position: absolute;
			bottom: -500px;
			left: -300px;
			content: '';
			width: 200%;
			height: 100vh;
			background-color: var(--background);
			filter: blur(100px);
		}

		& .content-readline-text-box {
			display: flex;
			flex-direction: column;
			z-index: 10;
			position: absolute;
			top: 50%;
			transform: translateY(-50%);
			width: 48%;
			padding: 0 5%;
		}
	}

	@media (max-width: 920px) {
		.readline-home-page {
			background-position: right;
		}

		.content-readline-text-box {
			width: 80% !important;
		}
	}

	@media (max-width: 720px) {
		.content-readline-text-box {
			width: 100% !important;
			text-align: center;
		}

		.content-readline-text-box p {
			font-size: 1.3rem;
		}

		.buttons-content-readline button {
			width: 100% !important;
		}

		.budget {
			display: none !important;
		}
	}
</style>
