<script lang="ts">
	import Navbar from '../../components/landing/Navbar.svelte';
	import Footer from '../../components/landing/Footer.svelte';
</script>

<Navbar />

<div class="wrapper">
	<section class="section-hero">
		<h2 style="text-align: center; margin-bottom: 5px;">Togo Water Campaign begins <br /> Sept 17, 2024</h2>
		<!-- <h5><em>Last updated: Monday 25 3:23pm PDT</em></h5> -->
		<br /><br />
		<h1 id="hero-heading">Welcome, Quirkies!</h1>
		<p style="margin-top:5px">
			<img src="/images/quirks.png" alt="Quirkies" class="responsive-image"/>
		</p>

		<h2>Impact Stream is partnering with Quirkies to raise $25k+ USD</h2>
		<br /><br />
		<h4>Donations help local entrepreneurs build two solar-powered wells in Togo, West Africa</h4>

		<p style="margin-top:5px">
			<img src="/images/well-locations.png" alt="Well Locations" class="responsive-image"/>
			
		</p>

		<div style="margin-top: -50px;">
			One well is for a village (marker on the right) called KLIKAME
  	</div>

		<br /><br />
		<h4>The other well is for an orphanage (marker on the left) in AMOUZOU-KOPE. They graciously shared this photo with us, knowing that we are doing our best to help.</h4>

		<p style="margin-top:5px">
			<img src="/images/orphanage.jpg" alt="Orphanage" class="responsive-image"/>
		</p>		

		<div>
			<h1>More Details</h1>
		</div>
		<br /><br />
		<p style="font-size: 18px;">
			See <a href="/">our home page</a> for a fuller description of what Impact Stream is all about and what we've accomplished in our first pilot round.
		</p>

		<p style="font-size: 18px;">
			TL;DR; We've helped people in Togo fund their top six voted projects for public goods. We initially raised $60k USD from friends and family, which allowed us to fund these projects. Projects #7 and #8 are the wells described above. We are partnering with Quirkies to make these projects come to life. 
		</p>

		<p style="font-size: 18px;">
			IMPORTANTLY, we have already built a well (Project #4) with the local entrepreneurs (who we know). Here are a couple recent videos of that process:
		</p>	

		<div class="video-container">
			<div class="video-wrapper">
					<iframe src="https://www.youtube.com/embed/_bGYlnGL-Xc?rel=0" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
			</div>      
			<div class="video-wrapper">
					<iframe src="https://www.youtube.com/embed/zk65Fg65OWs?rel=0" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
			</div>
	</div>

	<br />

		<p style="font-size: 18px;">
			Therefore, we are EXCITED to partner with the Quirkies community for this special campaign to fund these two additional wells!</p>
			
		<p style="font-size: 18px;">Please give via the form below and/or directly to impactstream.eth on Ethereum mainnet <em>(ETH, USDC, or USDT preferred, but we'll happily accept any token you'd be willing to donate)</em>. 
		</p>
		
		<p>THANK YOU! 🙏</p>

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

	.responsive-image {
    max-width: 100%;
    height: auto;
  }
	@media (min-width: 600px) {
    .responsive-image {
        margin-top: 10px; 
				margin-bottom: 10px;
    }
  }		

	section .value-prop-right {
    display: flex;
    flex-direction: column;
    align-items: center; 
	}	
	
	.video-container {
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 100%;
        max-width: 960px;
        margin: 0 auto;
    }

    .video-wrapper {
        position: relative;
        width: 100%;
        padding-bottom: 56.25%; /* 16:9 Aspect Ratio */
        height: 0;
        overflow: hidden;
        margin-bottom: 15px;
    }

    .video-wrapper iframe {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        border: 0;
    }	
</style>
