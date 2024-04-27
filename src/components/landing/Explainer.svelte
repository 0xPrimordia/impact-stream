<div class="content-wrapper">
	<section id="qv">
		<div class="value-prop-left">
			<img src="/images/vote.svg" alt="phone with voting options" />
		</div>
		<div class="value-prop-right">
			<h1>What is Quadratic Voting?</h1>
			<p>
				Quadratic Voting (QV) is a democratic decision-making system designed to more accurately reflect the strength of individuals' preferences on various issues compared to traditional voting methods. Under this system, voters are allocated a fixed number of credits, which they can use to cast votes on a range of proposals. The cost of each additional vote for a particular option increases quadratically, meaning the second vote costs more credits than the first, the third vote even more, and so on. This mechanism encourages voters to truly weigh their preferences, allowing them to express not just which options they favor but how strongly they feel about them. Quadratic Voting aims to minimize the influence of majority power while amplifying minority voices, providing a more nuanced and equitable assessment of collective priorities.
			</p>
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
	section .value-prop-right {
		display: flex;
		flex-direction: column;
		margin-top: 2em;
	}
	section .value-prop-left img {
		margin-top: 4em;
		margin-right: 4em;
	}
	section div a {
		text-decoration: none;
		color: #3e5f72;
		font-weight: bold;
		max-width: 18%;
	}

	section div a:hover {
		border-bottom: 2px solid #3e5f72;
	}
	@media (max-width: 600px) {
		.content-wrapper section {
			flex-direction: column;
		}
		section .value-prop-left img {
			margin: auto;
		}
		.value-prop-left {
			text-align: center;
		}
	}
	section h1 {
		margin-bottom: 5px;
	}		
</style>
