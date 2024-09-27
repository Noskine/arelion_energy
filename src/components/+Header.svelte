<script>
	import src from '$lib/images/logoAlternativo.png';
</script>

<header>
	<section>
		<img class="logotype" {src} alt="logotype alternative" />
	</section>
	<menu>
		<ul>
			<li><a href="/">Sobre nós</a></li>
			<li><a href="/">Sustentabilidade</a></li>
			<li><a href="/">Mobilidade Elétrica</a></li>
			<li><a href="/">Simulação de economia</a></li>
		</ul>
	</menu>
</header>

<style>
	header {
        line-height: 10px;
		padding-inline: 5%;
		display: flex;
		align-items: center;
		justify-content: space-between;


		& menu ul {
			list-style: none;
			display: flex;
			align-items: center;
			gap: 10px;

			& li {

                & > a {
					font-size: 1.4rem;
                    text-decoration: none;
				}
			}
		}
	}

	.logotype {
		width: 120px;
	}
</style>
