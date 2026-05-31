# How to setup Tailwind CSS

## Step 1: Create & Open Project Folder

- Create a folder named: math-mentor
- Open this folder in VS Code.

---

## Step 2: Initialize Vite

```
npm create vite@latest .
```

## Step 3: Selections:

- Framework: Vanilla  
- Variant: JavaScript  
- Install with npm: No

---

## Step 4: Some changes in src folder & index.html file

- Delete all files from "src" folder except "style.css" file
- Remove all content from "index.html" file

---

## STEP 5: Install tailwindcss and @tailwindcss/vite via npm.

```
npm install

npm install tailwindcss @tailwindcss/vite
```

## Step 6: Configure the Vite plugin

- Create vite.config.js file.
- Add the '@tailwindcss/vite' plugin to your Vite configuration.

```
import { defineConfig } from 'vite'
import tailwindcss from '@tailwindcss/vite'

export default defineConfig({
  plugins: [
    tailwindcss(),
  ],
})
```
