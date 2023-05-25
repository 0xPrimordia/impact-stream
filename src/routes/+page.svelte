<script lang="ts">
	import Navbar from '../components/landing/Navbar.svelte';
	import Logo from '../components/landing/Logo.svelte';
	import Valueprop from '../components/landing/Valueprop.svelte';
	import Footer from '../components/landing/Footer.svelte';
	import Explainer from '../components/landing/Explainer.svelte';
	import About from '../components/landing/About.svelte';

	export let data;
</script>

<Navbar />
<div class="wrapper">
	<section class="section-hero">
		<h1 id="hero-heading">{data.hero.title}</h1>
		<p class="sub">{data.hero.sub}</p>
		<button class="anchor" on:click={() => (window.location.href="/#Donate")}>Donate</button>
	</section>
</div>
<Valueprop />
<About />
<Explainer />
<div class="wrapper">
	<section>
		<h1>Team</h1>
		<div class="team">
			<div class="member">
				<div class="avatar" />
				<div><h3>Alidra</h3></div>
			</div>
			<div class="member">
				<div style="background-image:url(/images/will.png)" class="avatar" />
				<div><h3>Will</h3></div>
			</div>
			<div class="member">
				<div class="avatar" />
				<div><h3>Laté</h3></div>
			</div>
			<div class="member">
				<div style="background-image:url(/images/zakk.png)" class="avatar" />
				<div><h3>Zakk</h3></div>
			</div>
			<div class="member">
				<div class="avatar" />
				<div><h3>Angela</h3></div>
			</div>
			<div class="member">
				<div style="background-image:url(/images/kevin.png)" class="avatar" />
				<div><h3>Kevin</h3></div>
			</div>
			<div class="member">
				<div style="background-image:url()" class="avatar" />
				<div><h3>Matt</h3></div>
			</div>
			<div class="member">
				<div style="background-image:url()" class="avatar" />
				<div><h3>Kevin</h3></div>
			</div>
			<div class="member">
				<div style="background-image:url()" class="avatar" />
				<div><h3>Rob</h3></div>
			</div>
		</div>
	</section>
</div>
<div class="wrapper">
	<section>
		<h1>Partners</h1>
		<div class="partner-logos">
			<Logo src="images/ilad-logo.svg" />
			<Logo src="images/supermodular-logo.svg" />
			<Logo src="images/prota-ventures-logo.svg" />
			<Logo src="images/gitcoin-logo.svg" />
			<Logo src="images/primordia-logo.svg" />
		</div>
	</section>
</div>
<Footer />

<style>
	.anchor {
		cursor: pointer;
	}
	.wrapper section {
		max-width: 960px;
		margin: auto;
		display: flex;
		flex-direction: column;
		align-items: center;
		padding: 2em 0;
	}
	section.section-hero {
		padding: 8rem 0;
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
		padding: 1rem 6rem;
		border-radius: 10px;
		font-size: 1.5rem;
		font-weight: bold;
	}
	.wrapper p.sub {
		text-align: center;
	}

	.wrapper section div {
		display: flex;
		justify-content: center;
		align-items: center;
		flex-wrap: wrap;
	}
	div.team {
		display: flex;
		flex-wrap: wrap;
		max-width: 600px;
	}
	div.team .member {
		margin: 2rem;
		display: block;
		text-align: center;
	}
	div.team .member > div.avatar {
		width: 8rem;
		height: 8rem;
		background: #3e5f72;
		border-radius: 4rem;
		margin: auto;
		display: block;
	}


	div.partner-logos {
		display: flex;
		flex-wrap: wrap;
	}
	@media (max-width: 950px) {
		section.section-hero {
			padding: 4rem 0;
		}
		.wrapper section h1 {
			font-size: 2rem;
		}
		.wrapper section p {
			font-size: 1.5rem;
		}
		.wrapper section {
			padding: 2rem;
		}

	}
</style>
