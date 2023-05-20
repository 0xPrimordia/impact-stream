<script lang="ts">
	import Navbar from '../components/landing/Navbar.svelte';
	import Logo from '../components/landing/Logo.svelte';
	import Valueprop from '../components/landing/Valueprop.svelte';
	import Footer from '../components/landing/Footer.svelte';

	export let data;
</script>

<Navbar />
<div class="wrapper">
	<section>
		<h1 id="hero-heading">{data.hero.title}</h1>
		<p class="sub">{data.hero.sub}</p>
		<button>Donate</button>
	</section>
</div>
<Valueprop />
<div class="wrapper">
	<section>
		<h1>Explainer Section</h1>
		<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
	</section>
</div>
<div class="wrapper">
	<section>
		<h1>Team Section</h1>
		<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
	</section>
</div>
<div class="wrapper">
	<section>
		<h1>Partners</h1>
		<div>
			<Logo src="images/ilad-logo.svg" />
			<Logo src="images/supermodular-logo.svg" />
			<Logo src="images/prota-ventures-logo.svg" />
			<Logo src="images/gitcoin-logo.svg" />
			<Logo src="images/impact-stream-logo.svg" />
		</div>
	</section>
</div>
<Footer />

<style>
	.wrapper section {
		max-width: 960px;
		margin: auto;
		display: flex;
		flex-direction: column;
		align-items: center;
		padding: 6em 0;
	}

	.wrapper section h1 {
		font-size: 3rem;
		color: #3e5f72;
	}

	#hero-heading {
		color: #3e5f72;
	}
	.wrapper section p {
		font-size: 2rem;
		margin-bottom: 3rem;
	}

	.wrapper section button {
		background-color: #000;
		color: #ebf4e6;
		border: none;
		padding: 1rem 2rem;
		border-radius: 10px;
		font-size: 1.5rem;
		font-weight: bold;
		width: 33.3%;
	}
	.wrapper p.sub {
		text-align: center;
	}

	.wrapper section div {
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>
