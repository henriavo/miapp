<script>
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';

	import pinapple from '$lib/images/drawing-pineapple.webp';
	import pineapple_fallback from '$lib/images/drawing-pineapple.png';

	import pear from '$lib/images/pears-10.webp';
	import pear_fallback from '$lib/images/pears-10.png';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section id="pineapples">
	
	<span class="welcome">
		<picture>
			<source srcset={pinapple} type="image/webp" />
			<img src={pineapple_fallback} alt="pineapple" />
		</picture>
	</span>
	<span class="welcome">
		<picture>
			<source srcset={pinapple} type="image/webp" />
			<img src={pineapple_fallback} alt="pineapple" />
		</picture>
	</span>
	<span class="welcome">
		<picture>
			<source srcset={pinapple} type="image/webp" />
			<img src={pineapple_fallback} alt="pineapple" />
		</picture>
	</span>

	<h2>how many pinapples?</h2>
	<Counter />

	<div class="space"></div>

</section>

<section id="pears">

	<span class="welcome">
		<picture>
			<source srcset={pear} type="image/webp" />
			<img src={pear_fallback} alt="pear" />
		</picture>
	</span>
	<span class="welcome">
		<picture>
			<source srcset={pear} type="image/webp" />
			<img src={pear_fallback} alt="pear" />
		</picture>
	</span>
	<span class="welcome">
		<picture>
			<source srcset={pear} type="image/webp" />
			<img src={pear_fallback} alt="pear" />
		</picture>
	</span>
	<span class="welcome">
		<picture>
			<source srcset={pear} type="image/webp" />
			<img src={pear_fallback} alt="pear" />
		</picture>
	</span>

	<h2>how many pears?</h2>
	<Counter />
	
</section>

<div class="space"></div>

<section id="Features">
	<p>welcome to features</p>
</section>

<div class="space"></div>

<section id="Pricing">
	<p>welcome to pricing</p>
</section>

<div class="space"></div>

<style>
	.space { margin-top: 800px; }

	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	.welcome {
		display: block;
		position: relative;
		width: 50%;
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
