<script lang="ts">
	import { copy, type CopyDetail } from '@svelte-put/copy';
	import SocialIcons from '@rodneylab/svelte-social-icons';
	let ensButton: HTMLButtonElement;
	let addressButton: HTMLButtonElement;
	let ensIsClicked = false;
	let addressIsClicked = false;
	const handleEnsClick = () => {
		ensIsClicked = !ensIsClicked;
	};
	const handleAddressClick = () => {
		addressIsClicked = !addressIsClicked;
	};
</script>

<footer class="footer">
	<div class="ripple-line-blue" />
	<div id="Donate" class="donate">
		<div class="copy">
			<span>Your donation funds the building of public goods and IRL impact around the world.</span>
		</div>
		<div class="buttons">
			<button on:click={handleEnsClick} use:copy
				>impactstream.eth

				{#if ensIsClicked}
					<img src="/images/checkmark-icon.svg" alt="Check icon" class="check-icon" />
				{:else}<img src="/images/copy-icon.svg" alt="Copy icon" class="copy-icon" />
				{/if}</button
			>
			<span>I you don't have a crypto wallet, <a target="_blank" href="https://app.ribbon.giving/r/campaigns/camp_OAZVmcEnj0bnPVtS">donate at this link</a>.</span>
		</div>
	</div>
	<div class="ripple-border top" />
	<section>
		<div class="footer-cta">
			<div class="copy">
				<span>Join our community on Discord</span>
			</div>
			<div class="button-wrap">
				<button on:click={() => (window.location.href = 'https://discord.gg/we344V4QP7')}
					>Join Now</button
				>
			</div>
		</div>
		<div class="ripple-line" />
		<div class="bottom">
			<img src="/images/logo-small.png" alt="Impact Stream" />
			<div class="social-links">
				<a target="_blank" href="https://twitter.com/impact_stream"
					><SocialIcons network="twitter" fgColor="#ebe8cb" bgColor="rgba(105, 132, 146, 1)" /></a
				>
				<a target="_blank" href="https://discord.gg/we344V4QP7"
					><SocialIcons network="discord" fgColor="#ebe8cb" bgColor="rgba(105, 132, 146, 1)" /></a
				>
			</div>
			<div class="footer-link"><a href="mailto:hello@impact.stream">hello@impact.stream</a></div>
		</div>
	</section>
</footer>

<style>
	footer.footer section {
		background: rgba(105, 132, 146, 1);
	}
	div.ripple-border {
		height: 40px;
		background: top center transparent url('/images/ripple-border.svg');
		background-size: cover;
	}
	div.ripple-line {
		background: top center transparent url('/images/ripple-line.svg') no-repeat;
		background-size: 100%;
		height: 40px;
	}
	div.ripple-line-blue {
		background: top center transparent url('/images/ripple-line-blue.svg') no-repeat;
		background-size: 100%;
		height: 40px;
	}
	footer.footer .bottom {
		display: flex;
		align-items: center;
		padding-left: 2em;
	}
	footer.footer .bottom img {
		width: 2em;
		height: 2em;
	}
	div.footer-link {
		text-align: right;
		line-height: 2;
		padding: 2em;
		font-size: 0.9em;
		margin-left: auto;
	}
	div.footer-link a {
		color: white;
		text-decoration: none;
	}
	div.footer-link a:hover {
		text-decoration: underline;
	}
	.footer-cta {
		display: flex;
		padding: 2em;
		max-width: 960px;
		margin: auto;
		align-items: center;
	}
	.footer-cta .copy {
		font-size: 2em;
		font-weight: bold;
		color: #ebe8cc;
	}
	.donate {
		display: flex;
		max-width: 960px;
		margin: auto;
		padding: 4em 0;
	}
	.donate .copy {
		font-size: 2em;
		font-weight: bold;
		color: #3e5f72;
	}
	.donate .buttons {
		display: flex;
		flex-direction: column;
		margin-left: auto;
	}
	.buttons button {
		background: #3d5e71;
		border-radius: 15px;
		color: rgba(234, 232, 206, 1);
		font-size: 1em;
		border: none;
		font-weight: bold;
		padding: 1em 3em;
		line-height: 2rem;
	}
	.buttons button .copy-icon {
		width: 1.5em;
		height: 1.5em;
		position: relative;
		top: 0.2em;
		left: 0.2em;
	}

	.buttons button .check-icon {
		width: 1.5em;
		height: 1.5em;
		position: relative;
		top: 0.2em;
		left: 0.2em;
	}
	.buttons button:first-of-type {
		margin-bottom: 1.5em;
	}

	.buttons button:hover {
		color: rgba(105, 132, 146, 0.5);
	}
	.footer-cta button {
		background: #ebe8cb;
		border-radius: 5px;
		color: rgba(105, 132, 146, 1);
		font-size: 1em;
		border: none;
		font-weight: bold;
		padding: 1em 3em;
	}
	.footer-cta .button-wrap {
		margin-left: auto;
	}
	.social-links {
		margin-left: auto;
	}
	@media (max-width: 950px) {
		.donate {
			padding: 2rem;
		}
	}
	@media (max-width: 600px) {
		.footer-cta .copy {
			font-size: 1rem;
		}
		.donate {
			flex-direction: column;
		}
		.donate .copy {
			font-size: 1rem;
			text-align: center;
			margin-bottom: 2rem;
		}
		.donate .buttons {
			margin-left: 0;
		}
	}
</style>
