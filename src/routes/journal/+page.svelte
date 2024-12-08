<script>
	import HamburgerNavbar from '../../components/HamburgerNavbar.svelte';
</script>

<HamburgerNavbar title="Learning Journal" />

<h1>De journal van alle sprints</h1>
<div class="image">
<img src="./sprint.gif" alt="person running" width="200px">
</div>
<section class="journal">
	<a href="sprint13w1">
		<h2>Sprint 13, week 1</h2>
		<p>In week 1 hebben we SvelteKit geïnstalleerd en de basisprincipes geleerd. We ontdekten het verschil tussen Svelte en SvelteKit. We bestudeerden de structuur van een SvelteKit-project en leerden hoe we Directus kunnen integreren om data te ophalen.</p>
	</a>

	<a href="sprint13w2">
		<h2>Sprint 13, week 2</h2>
		<p>In week 2 werkten we verder aan de squadpage en kregen we een workshop over Figma. We leerden handige shortcuts voor een efficiënter ontwerp. Ook onderzochten we verschillende technieken om snel te werken in Figma.</p>
	</a>
	<a href="sprint13w3">
		<h2>Sprint 13, week 3</h2>
		<p>Week 3 stond in het teken van prioriteren met de MoSCoW-methode. We leerden hoe we user stories konden schrijven om de behoeften van gebruikers vast te stellen. De week werd afgesloten met een wrap-up van de sprint en een expo van de squadpage.</p>
	</a>
	<a href="sprint14w1">
		<h2>Sprint 1, week 1</h2>
		<p>Week 3 stond in het teken van prioriteren met de MoSCoW-methode. We leerden hoe we user stories konden schrijven om de behoeften van gebruikers vast te stellen. De week werd afgesloten met een wrap-up van de sprint en een expo van de squadpage.</p>
	</a>
	<a href="sprint14w2">
		<h2>Sprint 14, week 2</h2>
		<p>Week 3 stond in het teken van prioriteren met de MoSCoW-methode. We leerden hoe we user stories konden schrijven om de behoeften van gebruikers vast te stellen. De week werd afgesloten met een wrap-up van de sprint en een expo van de squadpage.</p>
	</a>
	<a href="sprint13w3">
		<h2>Sprint 14, week 3</h2>
		<p>Week 3 stond in het teken van prioriteren met de MoSCoW-methode. We leerden hoe we user stories konden schrijven om de behoeften van gebruikers vast te stellen. De week werd afgesloten met een wrap-up van de sprint en een expo van de squadpage.</p>
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

	.image {
        display: flex;
        justify-content: center;
        align-items: center;
    }
</style>
