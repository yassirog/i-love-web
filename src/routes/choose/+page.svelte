<script>
	import HamburgerNavbar from '../../components/HamburgerNavbar.svelte';
</script>

<HamburgerNavbar title="Learning Journal" />

<h1>De journal van alle sprints</h1>
<section class="journal">
	<a href="about">
		<p>Overmij</p>
	</a>

	<a href="journal">
		<p>de enige echte journal.</p>
	</a>
	<a href="we-love-web">
		<p>alle we-love-webs</p>
	</a>
</section>

<style>
	:root {
		color-scheme: dark;

		--green: 0, 255, 0;
		--white: 255, 255, 255;

		--primary-rgb: var(--green);
		--primary: rgb(var(--primary-rgb));
		--background: rgb(4, 4, 4);
		--background-light: rgba(var(--primary-rgb), 0.1);
		--background-hover: rgba(var(--primary-rgb), 0.4);
		--border: rgba(var(--primary-rgb), 0.2);
		--border-radius: 6px;
		--blur: blur(4px);
	}

	html,
	body {
		background-color: var(--background);
		margin: 0;
		padding: 0;
		box-sizing: border-box;
	}

	* {
		margin: 0;
	}

	h1 {
		font-family: Consolas, monospace, sans-serif;
		color: var(--primary);
		text-align: center;
		margin-top: 2em;
		margin: 1em;
	}

	.journal {
		display: flex;
		flex-direction: column;
		gap: 1em;
		padding: 1em;
		max-width: 800px;
		margin: 0 auto;
	}

	a {
		background-color: var(--background-light);
		border: 2px solid var(--border);
		border-radius: var(--border-radius);
		padding: 1em;
		backdrop-filter: var(--blur);
		color: var(--primary);
		transition:
			background-color 0.4s,
			border-color 0.4s;
	}

	a:hover {
		background-color: var(--background-hover);
		border-color: var(--primary);
	}

	a h2 {
		margin: 0 0 0.5em 0;
		font-family: Consolas, monospace, sans-serif;
		color: var(--primary);
	}

	a p {
		margin: 0;
		font-family: Consolas, monospace, sans-serif;
		color: var(--white);
	}

	a {
		text-decoration: none;
	}
</style>
