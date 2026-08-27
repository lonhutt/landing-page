# Lon Hutt — Portfolio & Consulting Website

This is the portfolio and consulting website for **Lon Hutt**, Principal Developer Productivity & Internal Platforms Consultant.

The site is built with modern, ultra-fast web tech to showcase technical expertise, consulting services, and recent developer experience (DevEx) achievements.

## 🛠️ Stack

- **Framework**: [Astro v5](https://astro.build/) (Static Site Generation)
- **Styling**: [Tailwind CSS v4](https://tailwindcss.com/) (modern CSS-first theme configuration)
- **Icons**: [Astro-Icon](https://github.com/natemoo-re/astro-icon) using `lucide` and `simple-icons` collections (standardized via Iconify)
- **Fonts**: Space Grotesk, Inter, and JetBrains Mono

## 📁 Project Structure

```text
/
├── public/
│   └── favicon.svg       # SVG favicon
├── src/
│   ├── components/
│   │   ├── About.astro          # About section
│   │   ├── Contact.astro        # Contact with links and Subject-prefilled email
│   │   ├── Hero.astro           # Header with title and main CTA button
│   │   ├── HeroSchematic.astro  # SVG animation showing pipeline optimization
│   │   ├── RecentWork.astro     # Project highlight/outcome section
│   │   └── WhatIDo.astro        # Focus offerings grid
│   ├── layouts/
│   │   └── Layout.astro         # Main HTML layout, fonts, and grid-paper texture
│   ├── pages/
│   │   └── index.astro          # Single-page entry combining sections
│   └── styles/
│       └── global.css           # Tailwind v4 import, custom theme tokens, animations
├── AGENTS.md                    # Environment-specific guidelines for AI assistants
└── package.json                 # Project dependencies and scripts
```

## 🧞 Development Commands

All commands are run from the root of the project:

| Command | Action |
| :--- | :--- |
| `npm install` | Installs dependencies |
| `npm run dev` | Starts local dev server at `localhost:4321` |
| `astro dev --background` | Starts dev server in background (managed with `astro dev stop`/`logs`) |
| `npm run build` | Builds the production site to `./dist/` |
| `npm run preview` | Previews the production build locally |
