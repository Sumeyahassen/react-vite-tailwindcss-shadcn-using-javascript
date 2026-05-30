# React + Vite + Tailwind CSS + shadcn/ui (JavaScript)

This project is built using React, Vite, Tailwind CSS, and shadcn/ui with JavaScript.

## 1. Create a Vite React Project

```bash
npm create vite@latest my-app -- --template react
cd my-app
npm install
```

## 2. Install Tailwind CSS

```bash
npm install tailwindcss @tailwindcss/vite
```

## 3. Configure Vite

Update `vite.config.js`:

```js
import { defineConfig } from 'vite'
import react from '@vitejs/plugin-react'
import tailwindcss from '@tailwindcss/vite'

export default defineConfig({
  plugins: [
    react(),
    tailwindcss(),
  ],
})
```

## 4. Configure Tailwind CSS

Update `src/index.css`:

```css
@import "tailwindcss";
```

## 5. Configure Import Aliases

Create a `jsconfig.json` file in the project root:

```json
{
  "compilerOptions": {
    "baseUrl": ".",
    "paths": {
      "@/*": ["./src/*"]
    }
  }
}
```

## 6. Initialize shadcn/ui

Run:

```bash
npx shadcn@latest init
```

When prompted, select:

```text
✔ Select a component library: Radix
✔ Which preset would you like to use?: Nova (Lucide / Geist)
```

## 7. Add Components

Example: Add a Button component.

```bash
npx shadcn@latest add button
```

## 8. Start the Development Server

```bash
npm run dev
```

## Project Stack

- React
- Vite
- Tailwind CSS
- shadcn/ui
- Radix UI
- Lucide Icons
- Geist Font

## Useful Commands

```bash
# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview

# Add shadcn components
npx shadcn@latest add button
npx shadcn@latest add card
npx shadcn@latest add input
npx shadcn@latest add dialog
```
