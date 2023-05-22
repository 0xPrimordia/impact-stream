<div>
	<div class="ripple-border top" />
	<div class="content-wrapper">
		<section>
			<div class="value-prop-left">
				<img src="/images/phone.svg" alt="phone with voting options" />
			</div>
			<div class="value-prop-right">
				<h1>On-Chain Quadratic Voting to Facilitate IRL Impact in Togo, West Africa</h1>
				<p>
					Cras fringilla dolor vitae justo pharetra, aliquet ultricies tortor aliquam. Maecenas sed
					ultricies nibh. Nullam ac pretium lorem, at tempor nulla. Pellentesque condimentum justo
					velit, et tempor libero suscipit et. Praesent placerat velit quis bibendum tristique. Duis
					sollicitudin ipsum id rhoncus auctor.
				</p>
				<p>
					Proin nec viverra est, in bibendum ex. Suspendisse bibendum porttitor viverra. Vestibulum
					placerat dui vitae accumsan tempor. Nam tempus tortor sit amet lorem aliquam, et molestie
					enim feugiat. Suspendisse non dui massa. Proin commodo est nec libero bibendum volutpat
					vitae nec ante. Nunc placerat lectus in placerat malesuada.
				</p>
				<p>
					Praesent placerat velit quis bibendum tristique. Duis sollicitudin ipsum id rhoncus
					auctor. Proin nec viverra est, in bibendum ex. Suspendisse bibendum porttitor viverra.
				</p>
				<button type="button" disabled>Coming Soon</button>
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
</style>

