# Astro Starter Kit: Basics

```sh
npm create astro@latest -- --template basics
```

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |


## Architecture

- **Entry point**: `src/pages/index.astro` - Main page composing all sections
- **Layout**: `src/layouts/Layout.astro` - Base layout with Header, Background, and MetaLayout
- **Components**: `src/components/` - Feature components (Presentation, Experience, Projects, Skills, Footer, Header, Background)
- **UI Components**: `src/components/ui/` - Reusable components (Card, Chip, SocialPill)
- **Icons**: `src/icons/` - Technology/brand icon components (each is an Astro component)
- **Models**: `src/models/enums.ts` - TypeScript enums for type safety
- **lib**: `src/lib/` - Utility libraries (e.g., `supabase.ts` for Supabase client)

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   └── Card.astro
│   ├── layouts/
│   │   └── Layout.astro
│   └── pages/
│       └── index.astro
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

Any static assets, like images, can be placed in the `public/` directory.

