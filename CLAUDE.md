# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Hipp AI landing page - a static marketing website for an AI automation consulting business. No build tools or dependencies required.

## Live Site

- **Production URL:** https://hippaihq.com
- **Vercel URL:** https://hipp-ai-website.vercel.app

## Deployment

The site auto-deploys via Vercel when changes are pushed to GitHub.

**Workflow:** Edit locally → `git push` → Vercel auto-deploys → Live on hippaihq.com

**GitHub repo:** https://github.com/dillonhippensteel/hipp-ai-website

## Development

To view the site locally, open `index.html` in a browser. No server or build step needed.

## Architecture

- **index.html** - Single-page structure with sections: Hero, Services, How It Works, About, CTA, Footer
- **styles.css** - CSS custom properties for theming (dark theme with neon green accent `#39FF14`), responsive breakpoints at 968px, 768px, 480px
- **script.js** - Vanilla JS for scroll-based nav styling, smooth anchor scrolling, and intersection observer fade-in animations

## Design System

- Fonts: Space Grotesk (headings), Inter (body)
- Primary color: `--color-primary: #39FF14` (neon green)
- Background: `--color-bg: #000000` (black)
- All interactive elements have hover states with glow effects

## Placeholders

Comments marked `CALENDLY_PLACEHOLDER` in index.html indicate where to replace `#contact` links with a Calendly scheduling URL when ready.

## Screenshots

Save screenshots to `screenshots/` folder for Claude Code to analyze. This folder is gitignored (not uploaded to GitHub).

## Contact

Business email: dillon@hippaihq.com
Domain registrar: Namecheap
Hosting: Vercel (connected to GitHub)
