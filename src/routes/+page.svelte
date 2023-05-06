<script>
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<!--h1>
		<span class="welcome">
			<picture>
				<source srcset={welcome} type="image/webp" />
				<img src="https://vonzimmermann.ch/wordpress/wp-content/uploads/2020/03/78146141_100743011417800_8369211781662375936_n-300x300.jpg" alt="Welcome" />
			</picture>
		</span>

		to your new<br />SvelteKit app
	</h1>

	<h2>
		try editing <strong>src/routes/+page.svelte</strong>
	</h2-->
	<h1>
		<a href="https://opensea.io/assets/ethereum/0x495f947276749ce646f68ac8c248420045cb7b5e/19155244552528182956849231716991578859342481968898501192175010786946555314177" target="_blank"><u>Click here to buy this image as NFT for only 0.22 ETH!</u></a>
	</h1>
	<a href="https://opensea.io/assets/ethereum/0x495f947276749ce646f68ac8c248420045cb7b5e/19155244552528182956849231716991578859342481968898501192175010786946555314177" target="_blank"><img style="width:50%" src="https://i.seadn.io/gcs/files/dfcc33b066b9f3862a600eb832dab7c9.jpg?auto=format&w=1000" alt="Welcome" /></a>
	<!--Counter /-->
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	h1 {
		width: 100%;
	}

	.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
</style>
