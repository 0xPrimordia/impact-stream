<script>
	import Logo from './Logo.svelte';
</script>

<nav class="main-nav">
	<Logo src="images/impact-stream-logo.svg" />
	<ul class="nav-links">
		<li class="nav-item"><a href="/">Home</a></li>
		<li class="nav-item"><a href="/app">App</a></li>
		<li class="nav-item"><a href="/qf">Quadratic Funding</a></li>
		<li class="nav-item"><a href="/team">Team</a></li>
		<li class="nav-item"><a href="/partners">Partners</a></li>
		<li class="nav-item"><a href="/donate">Donate</a></li>
	</ul>
</nav>

<style>
	nav.main-nav {
		background: #cbe5f1;
		display: flex;
		justify-content: space-between;
		padding: 0 1.5rem;
		font-family: 'Inter';
		font-size: 1rem;
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
</style>
