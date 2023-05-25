<div>
	<div class="ripple-border top" />
	<div class="content-wrapper">
		<section id="app">
			<div class="value-prop-left">
				<img src="/images/phone.svg" alt="phone with voting options" />
			</div>
			<div class="value-prop-right">
				<h1>Current Project: On-Chain Quadratic Voting and Matching Pool in Togo, West Africa</h1>
				<p>
					We are building and deploying a software application that will onboard 100 Togolese into
					Web3, allow them to submit proposals for IRL public goods (wells for clean water, schools,
					clinics, entrepreneurial endeavors for economic growth, etc), and conduct quadratic voting
					on the proposals that are most meaningful to them.
				</p>
				<p>
					The old way of non-profit work often involves a charitable outsider trying to solve the
					problems of a struggling community. Although this is well meaning, we’ve created a better
					way. Using Gitcoin’s <span><a href="https://docs.allo.gitcoin.co/">Allo Protocol</a></span
					>
					and <span><a href="https://www.gitcoin.co/grants-stack">Grants Stack</a></span>, we
					empower local people to propose their own solutions to the struggles their community is
					facing, signal to donors which proposals are most desired, and then leverage local
					laborers and vendors to build and maintain the public goods that are funded.
				</p>
				
			</div>
		</section>
	</div>
	<div class="ripple-border bottom" />
</div>

<style>
	.ripple-border {
		height: 40px;
		background: top center transparent url('/images/ripple-border.svg');
		background-size: cover;
		opacity: 0.75;
	}
	.ripple-border.bottom {
		transform: scaleY(-1);
	}
	.content-wrapper {
		background: rgba(105, 132, 146, 0.75);
	}
	.content-wrapper section {
		max-width: 960px;
		margin: auto;
		min-height: 4em;
		padding: 2em;
		display: flex;
	}
	section h1 {
		color: #f9ffe9;
		font-size: 2em;
		margin-bottom: 0;
	}
	section p {
		color: #fff;
		font-size: 1em;
	}
	section .value-prop-right {
		display: flex;
		flex-direction: column;
	}

	section div button {
		background: #ebe8cb;
		border-radius: 5px;
		color: rgba(105, 132, 146, 1);
		font-size: 1em;
		border: none;
		font-weight: bold;
		padding: 1em 4.5em;
		margin-top: 1.5em;
		align-self: flex-end;
	}

	section div button:disabled {
		background: #ebe8cb;
		color: rgba(105, 132, 146, 0.5);
		cursor: not-allowed;
	}

	section div img {
		margin-top: 3em;
		margin-right: 6em;
	}

	p span a {
		text-decoration: none;
		color: #cbe5f1;
	}

	p span a:hover {
		border-bottom: 1px solid #3e5f72;
	}
	@media (max-width: 600px) {
		.content-wrapper section {
			flex-direction: column;
		}
		div.value-prop-left {
			text-align: center;
		}
		section div img {
			margin: 0;
		}
	}
</style>
