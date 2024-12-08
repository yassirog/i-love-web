<script>
	import HamburgerNavbar from '../../components/HamburgerNavbar.svelte';
  </script>
  

<HamburgerNavbar title="Learning Journal"/>

<div class="wrapper">
	<div class="container"></div>

	<div class="components">
		<h1>About</h1>
		<img src="./pepe.gif" alt="hacker meme" width="200px">

		<div class="text-block">
			<p>
				Hoi, ik ben Yassir Bghiel, 20 j44r 0ud en kom uit W0erden. In m1jn vr13 t1jd ben ik vaak
				b3zig met twee d1ng3n waar ik veel p4ss13 voor heb: f1tn3ss en c0d3r3n. F1tn3ss h3lp+ m3 om
				fys13k en m3nt44l sterker te w0rden, en ik daag m3zelf gr4ag uit om st3eds b3t3r te w0rden.
				C0d3r3n is m1jn tw44d4 h0bb9. Ik h0ud ervan om m3zelf uit te d4g3n met c0d3rpr0bl3m3n,
				nieuwe t3chn0l0g13n t3 l3rn3n en pr0j3cts t3 b0uden w4ar ik trots op b3n.
			</p>
		</div>
	</div>
</div>

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
		box-sizing: border-box;
	}

	.wrapper {
		font-family: Consolas, monospace, sans-serif;
	}

	.container {
		height: 100%;
	}

	p {
		color: var(--primary);
		margin: 0;
	}

	.components {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		width: 100%;
	}

	h1 {
		margin-top: 3em;
		color: var(--primary);
		font-size: 32px;
	}

	.text-block {
		margin-top: 5em;
		max-width: 50ch;
		margin: 20px auto;
		padding: 10px;
		max-width: 1200px;
		backdrop-filter: blur(1.2px);
		border: 2px solid transparent;
		border-radius: 6px;
		text-wrap: wrap;
		transition: border-color 0.4s;
	}

	.text-block:hover {
		border-color: var(--border);
	}

	.text-block p {
		margin: 0;
		text-align: justify;
		color: var(--primary);
	}

	.btn-default {
		margin: 20px;
		padding: 10px 20px;
		backdrop-filter: var(--blur);
		background-color: var(--background-light);
		border: 2px solid var(--border);
		border-radius: var(--border-radius);
		color: var(--primary);
		font-size: 18px;
		font-family: Consolas, monospace, sans-serif;
		font-weight: bold;
		cursor: pointer;
		transition:
			background-color 0.4s,
			border-color 0.4s,
			backdrop-filter 0.4s;
	}

	.btn-default:hover {
		background-color: var(--background-hover);
		border-color: var(--primary);
	}
</style>
