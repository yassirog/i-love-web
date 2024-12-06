<div class="wrapper">
    <div class="container">
      <div class="letters" />
    </div>
    <div class="components">
      <h1>
        Learning Journal
      </h1>

      <div class="text-block">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
      </div>
      <button class="btn-default">
        Click Me
      </button>
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

body {
  background-color: var(--background);
  overflow: hidden;
}

.wrapper {
  font-family: Consolas, monospace, sans-serif;
}

.container {
  overflow: hidden;
  height: 100%;
}

.components {
  position: absolute;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 100%;
}

h1 {
  color: var(--primary);
  font-size: 36px;
}

.text-block {
  margin: 20px auto;
  padding: 10px;
  max-width: 1200px;
  backdrop-filter: blur(1.2px);
  border: 2px solid transparent;
  border-radius: var(--border-radius);
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
  transition: background-color 0.4s, border-color 0.4s, backdrop-filter 0.4s;
}

.btn-default:hover {
  background-color: var(--background-hover);
  border-color: var(--primary);
}

  </style>