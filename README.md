# Portfolio

The source code of my personal portfolio website, [dionaidan.com](https://dionaidan.com). It introduces me, lists my experience, projects, skills and education, and offers my CV for download.

## Features

- **Bilingual (Dutch and English)**: the language defaults to the visitor's browser setting, the choice is remembered, and the CV download follows the chosen language.
- **Single-page layout** with sections for about, experience, projects, skills, education and contact.
- **Content in one place**: all text lives in `constants/content.ts`, so updating the site means editing one typed file.
- **SEO and sharing basics**: generated sitemap, `robots.txt`, favicon and Open Graph image.
- **Accessibility**: semantic markup and keyboard-friendly navigation.
- **Privacy-friendly analytics** with Vercel Analytics.

## Tech stack

- Next.js 16 (App Router) and React 19
- TypeScript
- Tailwind CSS 4
- Biome for linting and formatting
- Deployed on Vercel

## Project structure

```
src/app/         Routes, layout, global styles, sitemap, robots, icon and OG image
components/      Navbar, Section, Tag
constants/       content.ts, the typed content for both languages
public/          CV PDFs (Dutch and English)
```

## How to run

**Requirements:** Node.js 20 or newer.

```bash
git clone https://github.com/verkerkaidan/portfolio.git
cd portfolio
npm install
npm run dev
```

Open http://localhost:3000.

Other scripts:

```bash
npm run build    # production build
npm run start    # serve the production build
npm run lint     # Biome checks
npm run format   # Biome formatting
```
