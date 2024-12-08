<script>
	import HamburgerNavbar from '../../components/HamburgerNavbar.svelte';
	import MarkdownRenderer from '../../components/MarkdownRenderer.svelte';

	// Je Markdown inhoud wordt hier dynamisch ingesteld
	let markdownContent = `
# Week 3
We zijn verder gegaan met het bouwen van de squadpage.
  
## 📅 Maandag - 16/09/2024
    We hebben een workshop gehad over prioriteren en het gebruik van de MoSCoW methode.
    Met User stories kan je aangeven in het algemeen en in detail wat je precies nodig hebt om het project
    af te maken en kan je je in het perspectief van de eindgebruiker plaatsen.
  
### User Stories
    \`\`\`
    Epic: In het algmeen beschrijven wat je ongeveer gaat bouwen.
    Stories: Globaal de functies beschrijven die je wilt bouwen.
    User Stories: Beschrijven in het perspectief van de gebruiker wat je wilt.
    Tasks: Specifiek taken gebasseerd op de user stories.
    \`\`\`
  
### MoSCoW methode
    \`\`\`
    Must Have: Dit zijn issues die moeten worden verwerkt in het project, zonder deze zal het project niet af zijn.
    Should Have: Dit zijn issues die het project verbeteren en eigenlijk wel verwerkt horen te worden. 
    Could Have: Dit zijn issues die het project meer verbeteren maar alleen worden verwerkt als er tijd over is.
    Would Have: Dit zijn extra issues met goed ideeën maar worden meestal niet verwerkt.
    \`\`\`
  
## 📅 Woensdag - 11/09/2024
    Wrap-up voor de sprint.
  
 ## 📅 Vrijdag - 13/09/2024
    Expo van de squadpage.
    `;
</script>

<HamburgerNavbar title="Learning Journal" />
<MarkdownRenderer {markdownContent} />
