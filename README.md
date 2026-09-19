# M A Rahman — Portfolio + Blog

Personal portfolio and blog for M A Rahman, Data Center Critical Infrastructure Electrical Engineer @ Amazon Web Services (AWS).

Built with [Astro](https://astro.build), deployed as a static site on Cloudflare Workers. Simple, flat black-and-white design, sharp corners, no shadows, Gentium Plus throughout.

## Pages

- `/` — M A Rahman. Portrait (clickable home), role, AWS link, LinkedIn / email / location contact lines, Professional Experience, Education, Projects, Certifications. Section headings collapse/expand with +/-.
- `/blog/` — My Blog. Compact portrait + name hero linking home, single post list.
- `/blog/[slug]` — Individual posts (Markdown Style Guide).

No About page. No social icons in header/footer. Footer: `2020 - 2026 — M A Rahman`.

## Project structure

- `src/pages/index.astro` — home portfolio
- `src/pages/blog/index.astro` — blog list with mini hero
- `src/pages/blog/[...slug].astro` — blog post route
- `src/content/blog/` — blog posts (Markdown Style Guide only)
- `src/components/Header.astro` — single `My Blog` tab
- `src/components/Footer.astro` — copyright + floating back-to-top arrow
- `src/layouts/BlogPost.astro` — flat black-and-white post layout
- `src/styles/global.css` — Gentium Plus, black/white, square, no shadows
- `public/mypic.jpg` — portrait
- `public/logos/` — AWS, Malloy, SDState, Starship, NUST, SKM, PIAIC
- `public/fonts/gentiumplus-*.ttf` — self-hosted Gentium Plus

## Commands

All commands run from the repo root:

| Command | Action |
| :------ | :----- |
| `npm install` | Installs dependencies |
| `npm run dev` | Starts local dev server at `localhost:4321` |
| `npm run build` | Builds production site to `./dist/` |
| `npm run preview` | Preview build locally before deploying |
| `npm run build && npm run deploy` | Deploy to Cloudflare Workers |

## Credit

Starter was the Astro blog template (Bear Blog base). Content, styling, and structure rebuilt for this portfolio.
