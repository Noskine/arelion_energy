<script>
	import Link from '$lib/components/cell/Link.svelte';
</script>

<section class="services">
	<div class="section-subtitle">
		<h2>Soluções solares que funcionam</h2>
		<small>Feito sob medida para a perfeição</small>
	</div>
	<hr />
	<section class="content-box-solutions">
		<div class="box-solutions">
			<h3>Instalação de Placas Solares</h3>
			<p>
				Soluções solares personalizadas, projetadas para atender às especificações exclusivas da sua
				casa ou empresa.
			</p>
			<Link href="/">Saiba mais</Link>
		</div>
		<div class="box-solutions">
			<h3>Soluções de armazenamento</h3>
			<p>
				Garanta energia ininterrupta com nossas soluções de armazenamento de bateria solar de última
				geração.
			</p>
			<Link href="/">Saiba mais</Link>
		</div>
		<div class="box-solutions">
			<h3>Auditoria de Eficiência</h3>
			<p>
				Maximize seu investimento com nossas auditorias abrangentes de eficiência solar, aprovadas
				pelo governo!
			</p>
			<Link href="/">Saiba mais</Link>
		</div>
		<div class="box-solutions">
			<h3>Financiamento e Incentivos</h3>
			<p>
				Navegue pelos aspectos financeiros de se tornar solar com facilidade. Isso inclui
				incentivos, descontos, subsídios e muito mais.
			</p>
			<Link href="/">Saiba mais</Link>
		</div>
	</section>
</section>

<style>

	hr {
		margin: 20px 0;
	}
	.services {
		padding: 40px 5%;

		& .section-subtitle {
			text-align: center;
			margin-bottom: 2.8rem;
		}

		& .content-box-solutions {
			display: grid !important;
			grid-template-columns: 1fr 1fr 1fr 1fr;
			width: 100%;
			gap: 20px;

			& .box-solutions {
				& h3 {
					font-weight: 700;
					font-size: 2rem;
					margin-bottom: 1rem;
				}

				& > p {
					font-size: 1.3rem;
				}
			}
		}
	}

	@media (max-width: 900px) {
		.content-box-solutions {
			grid-template-columns: 1fr 1fr !important;
		}
	}

	@media (max-width: 560px) {
		.content-box-solutions {
			grid-template-columns: 1fr !important;
		}
	}
</style>
