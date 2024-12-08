<script>
	import HamburgerNavbar from '../../components/HamburgerNavbar.svelte';
	import MarkdownRenderer from '../../components/MarkdownRenderer.svelte';

	// Je Markdown inhoud wordt hier dynamisch ingesteld
	let markdownContent = `
# Week 2
We werken verder aan het Deloitte project voor de opdrachtgever.

## 📅 Maandag - 30/09/2024
We hebben een workshop gehad over de structuur van Sveltekit en wat alles precies inhoud.

### Structuur
De structuur van Sveltekit is als volgt. (Dit is al in een andere journal vermeld)

- **app.html**: Dit bestand is de core van je project, het laad alles in om een pagina te tonen.
- **/routes**: Deze folder bevat alle routes van je project, deze map is verplicht in een Sveltekit project omdat het nodig is om een pagina te laden.
- **lib/server**: Deze folder is alleen voor server-side code zoals API_KEYS en/of wachtwoorden.
- **/static**: Deze folder bevat statisch bestanden die niet elke keer gebuild hoeven te worden door Sveltekit zoals afbeeldingen of een global.css bestand.
- **gitignore**: Dit bestand bevat informatie over delen code die je niet naar Github wil pushen.
- **package.json**: Dit bestand bevat alle nodige packages voor je project.
- **svelte.config**: Dit bestand bevat de configuratie van je Sveltekit project.
- **vite.config**: Dit bestand is een build tool voor je project.

### Routing
Voor frameworks wordt routing zelf ingesteld, je hoeft alleen een folder te creëren in de routes folder en dan wordt er een route voor aangemaakt.  
Je hebt 2 verschillende soorten routes: Static en Dynamic.  
- **Static route**: Een normale route met een naam van de route.  
- **Dynamic route**: Een route die een slug bevat oftewel een waarde die mee wordt gegeven vanuit een andere pagina, deze route heeft dus geen vaste naam zoals de static route maar past zich aan aan de waarde die wordt meegegeven.

### Error Handling
Met Sveltekit is het mogelijk om een error pagina te tonen als er bijvoorbeeld iets mis is met een bestand of de url van je pagina.  
Dit kan worden gedaan door in de routes folder een **+error.svelte** bestand aan te maken, wanneer de gebruiker op een niet bestaande pagina komt wordt hij verwezen naar dit bestand.  
Als je unieke error pagina's wil aanmaken voor elke route kan dat ook door het **+error.svelte** bestand te plaatsen in de folder van een route.  

Als Sveltekit niet werkt, kan je ook een **+error.html** bestand aanmaken in de src folder, deze pagina wordt alleen getoond als Sveltekit niet kan draaien voor de gebruiker.

### Layout
Als je pagina's hebt die hetzelfde layout gebruiken voor de structuur van een pagina, is het handig om een **+layout.svelte** bestand aan te maken.  
In dit bestand kan je een bepaald layout instellen die automatisch wordt toegepast op alle pagina's van je project.  
Dit doe je door het bestand in de routes folder te plaatsen, dit zorgt ervoor dat het op alle routes wordt toegepast.

### Loading Data
Om data in te laden vanuit Sveltekit kan je twee manieren gebruiken: **+page.js** en **+page.server.js**.  
Het verschil tussen deze twee bestanden is dat **+page.js** client-side is en **+page.server.js** server-side.

### Binding
Je kan met Sveltekit ook variabelen binden aan elementen waardoor je ze direct kan aanpassen.  
In dit voorbeeld heb je een **name** variabele met een waarde en een **shout** variabele die **name** combineert met een string.  
De **$:** voor de **shout** variabele zorgt ervoor dat het reactive wordt waardoor het in real-time aangepast wordt.  
Het **input** element heeft een **bind** attribuut die wordt verbonden aan de **name** variabele, dit zorgt ervoor dat wanneer je iets in het inputveld typt, de **name** variabele automatisch wordt aangepast op basis van wat jij typt.
`;

</script>

<HamburgerNavbar title="Learning Journal" />
<MarkdownRenderer {markdownContent} />
