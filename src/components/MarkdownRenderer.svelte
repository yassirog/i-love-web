<script>
    import { onMount } from 'svelte';
    import { marked } from 'marked';
    import createDOMPurify from 'dompurify';
  
    export let markdownContent = '';
  
    let renderedMarkdown = '';
  
    onMount(() => {
      if (typeof window !== 'undefined') {
        
        const DOMPurify = createDOMPurify(window);
        renderedMarkdown = DOMPurify.sanitize(marked(markdownContent));
      }
    });
  </script>
  
  <div class="markdown">
    {@html renderedMarkdown}
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
      padding: 0;
      box-sizing: border-box;
    }
  
    * {
      margin: 0;
    }
  
    .markdown {
      color: var(--primary);
      font-family: Consolas, monospace, sans-serif;
      padding: 1em;
      background-color: var(--background-light);
      border-radius: var(--border-radius);
      max-width: 1200px;
      margin: 2em auto;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
      backdrop-filter: var(--blur);
    }
  
    .markdown h1, .markdown h2, .markdown h3, .markdown h4, .markdown h5, .markdown h6 {
      color: var(--primary);
    }
  
    .markdown p {
      text-align: justify;
      margin: 0.5em 0;
      color: var(--primary);
    }
  
    .markdown ul, .markdown ol {
      margin: 1em 0;
      padding-left: 1.5em;
      color: var(--primary);
    }
  
    .markdown li {
      margin-bottom: 0.5em;
    }
  
    .markdown a {
      color: var(--green);
      text-decoration: none;
      transition: color 0.3s;
    }
  
    .markdown a:hover {
      color: var(--primary);
    }
  
    .markdown code {
      background-color: #2b2b2b;
      color: #fff;
      padding: 0.2em 0.4em;
      border-radius: 4px;
    }
  
    .markdown pre {
      background-color: #2b2b2b;
      color: #fff;
      padding: 1em;
      border-radius: 6px;
      overflow-x: auto;
      white-space: pre-wrap;
      word-wrap: break-word;
    }
  
    .markdown blockquote {
      border-left: 4px solid var(--primary);
      padding-left: 1em;
      color: var(--primary);
      font-style: italic;
    }
  
    .markdown hr {
      border: none;
      border-top: 1px solid var(--border);
      margin: 2em 0;
    }
  </style>
  