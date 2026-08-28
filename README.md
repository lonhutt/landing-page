# Lon Hutt — Portfolio & Consulting Website

This is the portfolio and consulting website for **Lon Hutt**, Principal Developer Productivity & Internal Platforms Consultant.

**Production site: [lonhutt.com](https://lonhutt.com)**

The site is built with modern, ultra-fast web tech to showcase technical expertise, consulting services, and recent developer experience (DevEx) achievements.

> The domain is configured as `site` in `astro.config.mjs`. It is the source for
> the canonical link, Open Graph URLs, and the JSON-LD `url` — change it there
> and every absolute URL follows.

## 🛠️ Stack

- **Framework**: [Astro v7](https://astro.build/) (Static Site Generation)
- **Styling**: [Tailwind CSS v4](https://tailwindcss.com/) (modern CSS-first theme configuration)
- **Icons**: [Astro-Icon](https://github.com/natemoo-re/astro-icon) using `lucide` and `simple-icons` collections (standardized via Iconify)
- **Fonts**: Space Grotesk, Inter, and JetBrains Mono — self-hosted and preloaded via Astro's built-in `fonts` config, so there is no render-blocking request to Google Fonts

## 📁 Project Structure

```text
/
├── public/
│   ├── favicon.ico       # Fallback favicon
│   ├── favicon.svg       # SVG favicon
│   ├── og-image.png      # 1200x630 social share card
│   └── robots.txt        # Crawler policy
├── src/
│   ├── components/
│   │   ├── About.astro          # About section
│   │   ├── BookCall.astro       # Shared "Book a call" CTA and calendar URL
│   │   ├── Contact.astro        # Contact links and closing CTA
│   │   ├── Hero.astro           # Header with title and main CTA button
│   │   ├── HeroSchematic.astro  # SVG animation showing pipeline optimization
│   │   ├── RecentWork.astro     # Project highlight/outcome section
│   │   ├── Section.astro        # Shared numbered-section shell (background, heading, rule)
│   │   └── WhatIDo.astro        # Focus offerings grid
│   ├── layouts/
│   │   └── Layout.astro         # Main HTML layout, fonts, SEO/OG meta, and grid-paper texture
│   ├── pages/
│   │   └── index.astro          # Single-page entry combining sections
│   └── styles/
│       └── global.css           # Tailwind v4 import, custom theme tokens, animations
├── AGENTS.md                    # Environment-specific guidelines for AI assistants
│                                # (CLAUDE.md is a symlink to it)
├── astro.config.mjs             # Site URL, font families, Tailwind + icon integrations
└── package.json                 # Project dependencies and scripts
```

Sections are composed with `Section.astro`, which takes an `index` and derives
the `[ 0N ]` counter and the alternating paper/paper-alt background from it, so
reordering or inserting a section needs no other edits.

## 🧞 Development Commands

All commands are run from the root of the project:

| Command | Action |
| :--- | :--- |
| `npm install` | Installs dependencies |
| `npm run dev` | Starts local dev server at `localhost:4321` |
| `astro dev --background` | Starts dev server in background (managed with `astro dev stop`/`logs`) |
| `npm run build` | Builds the production site to `./dist/` |
| `npm run preview` | Previews the production build locally |
