# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a personal portfolio website built with [Astro](https://astro.build). It showcases experience, projects, and skills.

## Commands

| Command           | Action                                           |
| :---------------- | :----------------------------------------------- |
| `npm run dev`     | Start local dev server at `localhost:4321`      |
| `npm run build`   | Run `astro check` and build to `./dist/`        |
| `npm run preview` | Preview the built site locally                 |
| `npm run astro`   | Run Astro CLI commands (e.g., `astro add`)      |

## Architecture

- **Entry point**: `src/pages/index.astro` - Main page composing all sections
- **Layout**: `src/layouts/Layout.astro` - Base layout with Header, Background, and MetaLayout
- **Components**: `src/components/` - Feature components (Presentation, Experience, Projects, Skills, Footer, Header, Background)
- **UI Components**: `src/components/ui/` - Reusable components (Card, Chip, SocialPill)
- **Icons**: `src/icons/` - Technology/brand icon components (each is an Astro component)
- **Models**: `src/models/` - TypeScript types (enums.ts, project.ts)
- **Data**: `src/lib/supabase.ts` - Supabase client for fetching dynamic content

The site uses a single-page layout with sections linked via anchor IDs (#about, #experience, #projects, #skills). Projects are fetched from Supabase at build time, while other content is defined in components.
