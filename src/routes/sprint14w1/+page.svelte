<script>
	import HamburgerNavbar from '../../components/HamburgerNavbar.svelte';
	import MarkdownRenderer from '../../components/MarkdownRenderer.svelte';

	// Je Markdown inhoud wordt hier dynamisch ingesteld
	let markdownContent = `
# Week 1
We zijn verder gegaan met het bouwen van de squadpage.

## 📅 Maandag - 23/09/2024
We zijn ingedeeld in groepen om een project te bouwen voor een opdrachtgever.
De opdrachtgever die ik heb gekregen is Drop and Heal.
Hiervoor hebben we een Team Canvas opgesteld en een Projectboard opgesteld
in de agency repository.

## 📅 Woensdag - 25/09/2024
?

## 📅 Vrijdag - 27/09/2024
Code/Design review`;
</script>

<HamburgerNavbar title="Learning Journal" />
<MarkdownRenderer {markdownContent} />
