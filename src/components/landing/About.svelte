<script lang="ts">
	import Logo from './Logo.svelte';
</script>

<div class="content-wrapper">
	<section id="#about">
		<div class="about-left">
			<h1>About Impact Stream</h1>
			<p>
				Overall, our mission is to create transparent, on-chain, and accountable impact between
				digital and IRL communities. Blockchains have ushered in new technology that allows anyone
				to observe verifiable transactions between known or anonymous people. Our goal is to
				level-up NGOs into web3; helping them leverage on-chain capabilities and operate
				transparently.
			</p>
			<p>
				When you give money to a traditional non-profit, you rarely have a way of knowing where
				exactly your money goes. You don’t how much goes to overhead and/or how much goes to the
				cause you care about. With Impact Stream, we encourage as many transactions as possible to
				occur on-chain to promote transparency. We envision this method becoming the gold standard
				for ethical non-profits around the globe. Our hope is to partner with digital communities -
				and especially web3 communities - who want to make an impact for the good of our planet and
				the flourishing of humanity.
			</p>
		</div>
		<div class="about-right">
			<Logo src="images/impact-stream-logo.svg" />
		</div>
	</section>
</div>

<style>
	.content-wrapper section {
		max-width: 960px;
		margin: auto;
		min-height: 4em;
		padding: 2em;
		display: flex;
	}
	section h1 {
		color: #3e5f72;
		font-size: 2em;
		margin-bottom: 0;
	}
	section p {
		color: #000;
		font-size: 1em;
		line-height: 1.5em;
		margin-bottom: 1em;
	}
	section .about-right {
		display: flex;
	}
	section .about-right img {
		margin-top: 3em;
		margin-left: 6em;
	}
	@media (max-width: 600px) {
		.content-wrapper section {
			flex-direction: column;
		}
		.about-right {
			text-align: center;
		}
		section .about-right img {
			display: none;
		}
	}
</style>
