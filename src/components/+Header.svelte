<script>
	import src from '$lib/images/logoAlternativo.png';
</script>

<header>
	<img class="logotype" {src} alt="logotype alternative" />
	<menu>
		<ul>
			<li><a href="/">Sobre nós</a></li>
			<li><a href="/">Sustentabilidade</a></li>
			<li><a href="/">Mobilidade Elétrica</a></li>
			<li><a href="/">Simulação de economia</a></li>
		</ul>
	</menu>
	<button id="contactUs"> Entre em contato </button>
</header>

<style>
	header {
		padding-inline: 5%;
		padding-block: 20px;
		display: flex;
		justify-content: space-between;
		align-items: center;
		background-color: #fff;
		box-shadow: var(--shadow);

		& menu {
			padding: 0;

			& ul {
				list-style: none;
				display: flex;
				align-items: center;
				gap: 15px;

				& li {
					& > a {
						font-size: 1.4rem;
						text-decoration: none;
						text-transform: capitalize;
						font-weight: 600;
						color: var(--color);
						transition: all 200ms;

						&:hover {
							color: var(--opaciteColor);
						}
					}
				}
			}
		}
	}

	.logotype {
		width: 150px;
		padding: 0;
	}

	#contactUs {
		border: none;
		font-size: 1.6rem;
		padding: 10px 15px;
		border-radius: 27px;
		color: #fff;
		font-weight: 700;
		cursor: pointer;

		background: rgb(77, 137, 255);
		background: -moz-linear-gradient(228deg, rgba(77, 137, 255, 1) 0%, rgba(98, 246, 235, 1) 100%);
		background: -webkit-linear-gradient(
			228deg,
			rgba(77, 137, 255, 1) 0%,
			rgba(98, 246, 235, 1) 100%
		);
		background: linear-gradient(228deg, rgba(77, 137, 255, 1) 0%, rgba(98, 246, 235, 1) 100%);
		transition: 10s ease-in-out;

		box-shadow: 0px 1px 4px 1px #00000026;
	}
</style>
