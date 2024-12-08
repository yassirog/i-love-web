<script>
	import HamburgerNavbar from '../../components/HamburgerNavbar.svelte';
</script>

<HamburgerNavbar title="Learning Journal" />

<h1>Overzicht van alle we-love-webs</h1>
<div class="image">
    <img src="./globe.gif" alt="globe spinning" width="200px">
    </div>
<section class="journal">
	<a href="talk2">
		<h2>Talk 2, Creative Developer</h2>
		<p>Een Creative Developer combineert creativiteit en technische vaardigheden om interactieve websites en applicaties te ontwerpen met tools zoals JavaScript, CSS en WebGL. Animaties en interacties moeten het verhaal ondersteunen, de gebruiker betrekken en technische uitdagingen oplossen.</p>
	</a>

	<a href="talk3">
		<h2>Talk 3, Portfolio</h2>
		<p>Bij het opzetten van een portfolio is het belangrijk om na te denken over het ontwerp, de inhoud en het doel ervan, en of je een oud portfolio kunt hergebruiken. Dion raadt aan om animaties toe te voegen voor een betere gebruikerservaring, maar vindt het niet noodzakelijk dat een designer kan coderen of andersom.</p>
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
