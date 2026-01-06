# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Hipp AI landing page - a static marketing website for an AI automation consulting business. No build tools or dependencies required.

## Development

To view the site, open `index.html` in a browser. No server or build step needed.

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

## Contact

Business email: dillon@hippaihq.com
