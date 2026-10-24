# Frontend Developer Portfolio

A modern, maintainable frontend developer portfolio foundation built with [Astro](https://astro.build/), [TypeScript](https://www.typescriptlang.org/), and [Tailwind CSS](https://tailwindcss.com/).

## Tech Stack

- **Framework**: Astro (Static site generation)
- **Styling**: Tailwind CSS (via `@tailwindcss/vite`)
- **Language**: TypeScript (Strict configuration)
- **Package Manager**: npm

## Architecture

The project structure is organized by responsibility to keep presentation, layout, and data separated:

```text
├── public/
│   ├── images/       # Static images and brand assets
│   └── projects/     # Static assets for portfolio project showcases
├── src/
│   ├── components/
│   │   ├── layout/   # Structural components (Navbar, Footer, etc.)
│   │   └── ui/       # Atomic/presentation components (Button, Badge, etc.)
│   ├── data/         # Structured content (projects, experience, skills data)
│   ├── layouts/      # Base HTML shells and page metadata layouts
│   ├── pages/        # Astro file-based routes
│   ├── styles/       # Global styles and Tailwind entry point
│   └── types/        # Shared TypeScript interfaces and type definitions
├── astro.config.mjs  # Astro and Vite plugin configuration (static output)
├── package.json      # Dependencies and scripts
└── tsconfig.json     # Strict TypeScript configuration extending Astro strict
```

## Available Scripts

| Command | Description |
| :--- | :--- |
| `npm install` | Installs project dependencies |
| `npm run dev` | Starts the Astro development server at `http://localhost:4321` |
| `npm run build` | Compiles the static production build into `./dist/` |
| `npm run preview` | Starts a local server to preview the production build |
| `npm run check` | Runs Astro diagnostic and TypeScript checks |
