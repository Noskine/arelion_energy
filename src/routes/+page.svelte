<script>
<<<<<<< HEAD
<<<<<<< HEAD
	import Readline from '$lib/components/Readline.svelte';
	import Services from '$lib/components/Services.svelte';
=======
	// import welcome from '$lib/images/svelte-welcome.webp';
>>>>>>> eef1d67f (starting new project)
=======
	import welcome from '$lib/images/Getty_1198580060-2798853475.jpg';
	import Icon from '@iconify/svelte';
	$: src = welcome;
>>>>>>> a6f83b12 (crate readLine)
</script>

<svelte:head>
	<title>Home</title>
</svelte:head>

<<<<<<< HEAD
<section>
<<<<<<< HEAD
	<Readline />
	<Services />
=======
	<h1>Olá mundo!</h1>
>>>>>>> eef1d67f (starting new project)
=======
<section id="home">
	<section id="readLine" style={`background-image: url(${src})`}>
		<section class="text-box">
			<span class="">Economize e invista no seu futuro!</span>
			<span class="title">Economize hoje e construa seu futuro com Aurelion Sol</span>
		</section>
	</section>
>>>>>>> a6f83b12 (crate readLine)
</section>

<style>
	#readLine {
		width: 100%;
		height: 75vh;
		background-repeat: no-repeat;
		background-size: 1100px;
		background-position: right;
		position: relative;
		overflow: hidden;
		z-index: -1;

		&::before {
			z-index: 0;
			content: '';
			position: absolute;
			background-color: var(--background);
			filter: blur(80px);
			left: -30%;
			width: 80%;
			height: 900px;
			top: 50%;
			transform: translateY(-50%);
		}
	}

	.text-box {
		width: 40%;
		display: flex;
		flex-direction: column;
		position: relative;
		top: 50%;
		gap: 5px;
		transform: translateY(-50%);
		padding-left: 5%;
	}

	.title {
		width: 100%;
		font-size: 4.2rem;
		line-height: 4.2rem;
		font-weight: 800;
	}
</style>
