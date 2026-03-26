# How to setup Tailwind CSS

---

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
- Add the @tailwindcss/vite plugin to your Vite configuration.

```
import { defineConfig } from 'vite'
import tailwindcss from '@tailwindcss/vite'

export default defineConfig({
  plugins: [
    tailwindcss(),
  ],
})
```

## Step 7: Import Tailwind CSS

- Add an @import to your CSS file that imports Tailwind CSS.

```
@import "tailwindcss";
```

## Step 8: Start your build process

```
npm run dev
```

## Step 9: Start using Tailwind in your HTML

```
<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="/src/style.css" rel="stylesheet">
</head>
<body>
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
</body>
</html>
```