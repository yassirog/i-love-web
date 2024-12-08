

<div class="wrapper">
	<div class="container"></div>

	<div class="components">
		<h1>W3lk0m!</h1>
		<img src="./hack.gif" alt="" width="200px">
		<div class="text-block">
			<p>
				Hallo en welkom op mijn (Yassir's) persoonlijke Learning Journal! Dit is de plek waar ik
				mijn leerproces, projecten en groei als Frontender documenteer. Hier deel ik mijn successen,
				uitdagingen en alles wat ik onderweg ontdek. Van nieuwe concepten en technieken tot
				creatieve projecten en reflecties op mijn voortgang, je vindt het allemaal hier. Mijn doel
				is niet alleen om mijn eigen ontwikkeling bij te houden, maar ook om te inspireren en kennis
				te delen met anderen die dezelfde reis maken.
			</p>
		</div>
		<a href="choose" class="btn-default"> Ga naar de kiespagina </a>
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

    html, body {
  background-color: var(--background);
  margin: 0;
  padding: 0; /* Zorg ervoor dat er geen padding is */
  box-sizing: border-box;
}

    * {
        margin: 0;
    }

    nav {
        display: flex;
        justify-content: space-between;
    }

	.wrapper {
		font-family: Consolas, monospace, sans-serif;
        margin: 1em;
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
