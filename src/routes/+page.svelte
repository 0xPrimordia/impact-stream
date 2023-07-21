<script lang="ts">
	import Navbar from '../components/landing/Navbar.svelte';
	import Logo from '../components/landing/Logo.svelte';
	import Valueprop from '../components/landing/Valueprop.svelte';
	import Footer from '../components/landing/Footer.svelte';
	import Explainer from '../components/landing/Explainer.svelte';
	import About from '../components/landing/About.svelte';


</script>


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
	div.team .member div.avatar {
		width: 8rem;
		height: 8rem;
		background: #3e5f72;
		background-size: 100% auto;
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

	@media (max-width: 376px) {
		.wrapper section h1 {
			font-size: 1.9rem;
		}
		.wrapper section p {
			font-size: 1.25rem;
		}
	}
</style>
