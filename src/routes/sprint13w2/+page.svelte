<script>
    import HamburgerNavbar from '../../components/HamburgerNavbar.svelte';
    import MarkdownRenderer from '../../components/MarkdownRenderer.svelte';
    
    // Je Markdown inhoud wordt hier dynamisch ingesteld
    let markdownContent = `
 # Week 2
    We zijn verder gegaan met het bouwen van de squadpage en hebben een workshop gehad over Figma.
  
## 📅 Maandag - 09/09/2024
    Vandaag hebben we een workshop gehad over Figma waar we diverse shortcuts hebben geleerd en verschillende
    manieren om snel en efficiënt een ontwerp te bouwen in Figma.
  
    Dit zijn handige shortcuts om sneller te werken met Figma.
    \`\`\`
    Move Tool: V
    Pen Tool: P
    Rectangle Tool: R
    Ellipse Tool: E
    Line Tool: L
    Frame Tool: F
    Copy: CTRL+C
    Paste: CTRL+P
    Group: CTRL+G
    Ungroup: CTRL+SHIFT+G
    Duplicate: CTRL+D
    Zoom-In: +
    Zoom-Out: -
    Equal Sizing: ALT
    \`\`\`
  
### Bronnen
    [Figma shortcuts](https://help.figma.com/hc/en-us/articles/360040328653-Keyboard-shortcuts-in-Figma)
  
## 📅 Woensdag - 11/09/2024
    We hebben een workshop gehad over creative coding.
  
## 📅 Vrijdag - 13/09/2024
    Code & Design review voor de squadpage.
    `;
  </script>
  
  <HamburgerNavbar title="Learning Journal" />
  
  <MarkdownRenderer {markdownContent} />
  