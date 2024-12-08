<script>
  export let title = "Learning Journal";
  
  let isMenuOpen = false; 
  
  function toggleMenu() {
    isMenuOpen = !isMenuOpen;
  }
</script>

<header class="header">
  <div class="title">
    <div class="title-row">
      <a href="/">
      <h1>{title}</h1>
    </a>
    </div>
  </div>

  <button class="hamburger" on:click={toggleMenu}>
    &#9776;
  </button>

  <div class="navigation-items {isMenuOpen ? 'open' : ''}">
    <a href="about" class="item">
      about
    </a>
    <a href="journal" class="item">
      journal
    </a>
    <a href="we-love-web" class="item">
      we love web
    </a>
  </div>
</header>

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

  header {
    width: 100%;
    border-bottom: 0.05px solid var(--primary);
    margin-bottom: 1em;
    margin: 0em;
    position: relative;
    font-family: Consolas, monospace, sans-serif;
  }

  .header {
    display: flex;
    margin-left: auto;
    justify-content: space-between;
    align-items: center;
  }

  p {
    color: var(--primary);
  }


  .title {
    margin: 1em;
  }

  .title-row {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
  }

  .title-row a {
    text-decoration: none;
  }

  .title-row h1 {
		font-family: Consolas, monospace, sans-serif;
    margin: 0;
    color: var(--primary);
  }


  /* Hamburger button */
  .hamburger {
    display: none;
    background: none;
    border: none;
    color: var(--primary);
    font-size: 30px;
    cursor: pointer;
    margin-right: 1em;
  }

  a {
    color: var(--primary);
		margin: 0;

  }

  .navigation-items {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    display: block;
  }

  .navigation-items.open {
    display: flex;
  }

  .item {
    display: flex;
    align-items: center;
    text-decoration: none;
    padding: 1em;
    color: var(--primary);
    margin-right: 20px;
    text-align: center;
    flex-direction: column;
    transition: 0.5s all;
    border: 2px solid transparent;
    border-radius: 5px; 
  }

  .item:hover {
    scale: 1.1;
  }

  /* Mobile - Hamburger Menu */
  @media (max-width: 1200px) {
    .hamburger {
      display: block;
    }

    .navigation-items {
      display: none;
      align-items: flex-start;
      height: 100%;
      width: 100%;
      position: absolute;
      top: 70px;
      left: 0;
      z-index: 10;
      margin: 0;
    }

    .navigation-items.open {
      display: flex;

    }

    .navigation-items .item {
      margin: 1em 0;
      width: 100%;
      text-align: left;
    }

    .navigation-items.open .item {
      border-bottom: 1px solid var(--primary);
      background-color: var(--background);
    }
  }

  @media (min-width: 1201px) {
    .navigation-items {
      display: flex;
      flex-wrap: wrap;
    }

    .item {
      margin: 0 1em;
      flex-direction: column;
      max-width: 10ch;
    }
  }
</style>
