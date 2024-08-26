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
		<button class="anchor" on:click={() => (window.location.href = '/#Donate')}>Donate</button>
	</section>
</div>
<Valueprop />
<About />
<Explainer />
<div class="wrapper">
	<section id="team">
		<h1>Team</h1>
		<div class="team">
			<div class="member">
				<a href="https://twitter.com/alidra_xyz" target="_blank"
					><div style="background-image:url(/images/alidra.jpeg)" class="avatar" /></a
				>
				<div><h3>Alidra</h3></div>
			</div>

			<div class="member">
				<a href="" target="_blank"
					><div style="background-image:url(/images/laté.png)" class="avatar" /></a
				>
				<div><h3>Laté</h3></div>
			</div>

			<div class="member">
				<a href="" target="_blank"
					><div style="background-image:url(/images/azaria.png)" class="avatar" /></a
				>
				<div><h3>Azaria</h3></div>
			</div>

			<div class="member">
				<a href="" target="_blank"
					><div style="background-image:url(/images/jacques.png)" class="avatar" /></a
				>
				<div><h3>Jacques</h3></div>
			</div>

			<div class="member">
				<a href="https://www.linkedin.com/in/itsmarkschubert/" target="_blank"
					><div style="background-image:url(/images/mark.jpeg)" class="avatar" /></a
				>
				<div><h3>Mark</h3></div>
			</div>	

			<div class="member">
				<a href="https://obertal.com/leavenworth-wa-hotel-owner/" target="_blank"
					><div style="background-image:url(/images/hans.png)" class="avatar" /></a
				>
				<div><h3>Hans</h3></div>
			</div>

			<div class="member">
				<a href="https://www.linkedin.com/in/wclittle/" target="_blank"
					><div style="background-image:url(/images/will.png)" class="avatar" /></a
				>
				<div><h3>Will</h3></div>
			</div>	

			<div class="member">
				<a href="https://twitter.com/princessashleiv" target="_blank"
					><div style="background-image:url(/images/ashlei.png)" class="avatar" /></a
				>
				<div><h3>Ashlei</h3></div>
			</div>	

			<div class="member">
				<a href="https://twitter.com/OneAndOnlyPapii" target="_blank"
					><div style="background-image:url(/images/papii.jpg)" class="avatar" /></a
				>
				<div><h3>Papii</h3></div>
			</div>				

			<div class="member">
				<a href="https://twitter.com/0xZakk" target="_blank"
					><div style="background-image:url(/images/zakk.png)" class="avatar" /></a
				>
				<div><h3>Zakk</h3></div>
			</div>

			<div class="member">
				<a href="https://www.linkedin.com/in/angela-angelovska-wilson-38600a1/" target="_blank"
					><div style="background-image:url(/images/angela.jpg)" class="avatar" /></a
				>
				<div><h3>Angela</h3></div>
			</div>
			<div class="member">
				<a href="https://www.linkedin.com/in/roy-nyaga-andre/" target="_blank"
					><div style="background-image:url(/images/roy.jpg)" class="avatar" /></a
				>
				<div><h3>Roy</h3></div>
			</div>			
			<div class="member">
				<a href="https://twitter.com/owocki" target="_blank"
					><div style="background-image:url(/images/kevin.png)" class="avatar" /></a
				>
				<div><h3>Kevin O</h3></div>
			</div>
			<div class="member">
				<a href="https://bento.me/captaincrunch" target="_blank"
					><div style="background-image:url(/images/captaincrunch.png)" class="avatar" /></a
				>
				<div><h3>Kevin C</h3></div>
			</div>
			<div class="member">
				<a href="https://twitter.com/sejal_rekhan" target="_blank"
					><div style="background-image:url(/images/sejal.jpeg)" class="avatar" /></a
				>
				<div><h3>Sejal</h3></div>
			</div>

		</div>
	</section>
</div>

<div class="video-container" style="margin-bottom: -75px">
	<iframe src="https://www.youtube.com/embed/FSXgJ3airoU?rel=0" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

<div class="wrapper">
	<section id="partners">
		<h1>Partners</h1>
		<div class="partner-logos">
			<Logo src="images/ilad-logo.svg" />
			<Logo src="images/supermodular-logo.svg" />
			<Logo src="images/prota-ventures-logo.svg" />
			<Logo src="images/gitcoin-logo.svg" />
			<Logo src="images/primordia-logo.svg" />
			<Logo src="images/cfx-black.svg" />			
			<Logo src="images/quirkies.png" />				
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

	.video-container {
        position: relative;
        padding-bottom: 56.25%; /* 16:9 aspect ratio */
        height: 0;
        overflow: hidden;
        max-width: 1200px; /* Set your desired max-width here */
        margin: 0 auto 15px auto; /* Center the video on the page */
    }

	.video-container iframe {
			position: absolute;
			top: 0;
			left: 0;
			width: 100%;
			height: 80%;
	}

</style>
