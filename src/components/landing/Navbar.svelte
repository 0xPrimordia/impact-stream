<script lang="ts">
	import Logo from './Logo.svelte';
	import { Icon, Bars2, XMark } from "svelte-hero-icons"
	let open:Boolean;
</script>

<nav class="main-nav">
	<Logo src="images/impact-stream-logo.svg" />
	<ul class={"nav-links" + (open ? ' hamburgle':'')}>
		<li class="nav-item"><a href="/">Home</a></li>
		<li class="nav-item"><a href="/#app">App</a></li>
		<li class="nav-item"><a href="/#qf">Quadratic Funding</a></li>
		<li class="nav-item"><a href="/#team">Team</a></li>
		<li class="nav-item"><a href="/#partners">Partners</a></li>
		<li class="nav-item"><a href="/#Donate">Donate</a></li>
	</ul>
	<span on:click={() => (open ? open=false:open=true)} on:keydown class="hamburgler">
		<Icon size="2rem" src={open ? XMark : Bars2} />
	</span>
</nav>

<style>
	nav.main-nav {
		background: #cbe5f1;
		display: flex;
		justify-content: space-between;
		padding: 0 1.5rem;
		font-family: 'Inter';
		font-size: 1rem;
		vertical-align: middle;
	}
	ul.nav-links {
		display: flex;
		list-style: none;
	}
	li.nav-item {
		display: inline-block;
		padding: 1.5rem;
	}
	.nav-item a {
		text-decoration: none;
		font-weight: bold;
		color: #000;
	}

	.nav-item a:hover {
		border-bottom: 2px solid #000;
	}
	span.hamburgler {
		display: none;
		margin-top:1.5rem;
		margin-right: 0.5rem;
		margin-left: auto;
		z-index: 555;
	}
	@media (max-width: 950px) {
		ul.nav-links {
			display: block;
			padding-top: 4rem;
			font-size: 1.5rem;
			position: fixed;
			background: #cbe5f1;
			right: 0;
			left: 0;
			top: 0;
			bottom: 0;
			margin: 0;
			z-index: 444;
			display: none;
		}
		ul.nav-links.hamburgle {
			display: block;
		}
		li.nav-item {
			display: block;
		}
		span.hamburgler {
			display: block;
		}
	}
</style>
