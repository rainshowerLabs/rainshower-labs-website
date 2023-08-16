<script>
	import logo from '$lib/images/logo.png';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
</script>


<svelte:head>
	<title>Home</title>
	<meta name="description" content="Rainshower Labs website" />
</svelte:head>

<section>
	<h1>
		<span class="logo">
			<picture>
				<source srcset={logo} type="image/webp" />
				<img src={welcome_fallback} alt="Rainshower Labs" />
			</picture>
		</span>

		Building what's next.
	</h1>

	<h2>
		Rainshower labs is focused on building the next evolution of DeFi, and tools that will make that happen.
	</h2>
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
		color: black;
	}

	.logo {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.logo img {
		position: absolute;
		width: 100%;
		height: 50%;
		top: 0;
		display: block;
	}
</style>
