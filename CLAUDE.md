# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Business Overview - Hipp AI LLC

**Founded:** January 1, 2026

**Mission:** Help companies implement AI into their business to help them grow, while building a profitable AI agency.

**Founder:** Dillon Hippensteel

### Business Model & Strategy

Target market: Companies hiring for roles that could be replaced/augmented by AI (a "starving market" - they're already spending money to solve this problem).

**Ideal Customer Profile:**
- Companies with 50-500 employees (big enough to have budget, small enough to make decisions quickly)
- Already hiring for positions that AI could handle
- Has buying power (budget already allocated for hiring)

**Influences & Principles:**
- Alex Hormozi's "$100M Offers" - focus on starving markets, irresistible offers
- "Atomic Habits" - systems and habit building
- "The E-Myth" - building systems, working ON the business not just IN it

### Current Lead Generation Workflow (n8n)

Built a workflow that:
1. Scrapes LinkedIn jobs that could be replaced by AI
2. Adds job/company info to CRM
3. Qualifies leads (50-500 employees filter)
4. Adds qualified leads to Google Sheet
5. Uses Apollo to enrich leads with employee contacts/emails
6. Goal: Send cold outreach emails → Book Zoom meetings → Close deals

**Status:** Workflow works through qualification, but cold email piece needs optimization.

**Next step:** Set up n8n MCP so Claude Code can help build and optimize workflows more efficiently.

---

## Website Project

Hipp AI landing page - a static marketing website for the AI automation consulting business. No build tools or dependencies required.

## Live Site

- **Production URL:** https://hippaihq.com
- **Vercel URL:** https://hipp-ai-website.vercel.app

## Deployment

The site auto-deploys via Vercel when changes are pushed to GitHub.

**Workflow:** Edit locally → `git push` → Vercel auto-deploys → Live on hippaihq.com

**GitHub repo:** https://github.com/dillonhippensteel/hipp-ai-website

**Note:** Ask the user if they want to push to GitHub after completing meaningful changes (features, fixes, updates).

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

## Calendly Integration

**Calendly URL:** https://calendly.com/dillon-hippaihq/ai-automation-strategy-call

Used for "Book a Call" and "Get Started" buttons throughout the site.

## AI Chatbot (COMPLETED Jan 7, 2026)

n8n-powered AI chatbot embedded on the website:

- **n8n Workflow:** "HIPP AI Customer Chatbot" (ID: 2ctxAFMcKu9kzVNJ)
- **Webhook URL:** https://dillonhippensteel12.app.n8n.cloud/webhook/hipp-ai-chat/chat
- **LLM:** OpenAI GPT-4o-mini (temperature 0.7)
- **Memory:** 10-message context window
- **Style:** Matches site design (black bg, neon green accents, Inter font)

**Chatbot Personality:**
- Follows Alex Hormozi C.L.O.S.E.R sales framework
- Value-focused, direct & confident communication
- Guides users toward discovery calls
- Has full HIPP AI service knowledge embedded in system prompt

**To update chatbot behavior:** Edit the system prompt in the AI Agent node in n8n.

## Screenshots

Save screenshots to `screenshots/` folder for Claude Code to analyze. This folder is gitignored (not uploaded to GitHub).

## n8n MCP Setup (COMPLETED Jan 6, 2026)

n8n MCP + Skills are fully configured:

- **n8n Instance:** https://dillonhippensteel12.app.n8n.cloud/
- **MCP Config:** `C:\Users\dillo\OneDrive\Desktop\Claude Code\.mcp.json`
- **Skills:** `C:\Users\dillo\.claude\skills\` (7 n8n skills installed)
- **Docs:** https://github.com/czlonkowski/n8n-mcp

To use: Start Claude Code from the `Claude Code` directory.

## Contact

Business email: dillon@hippaihq.com
Domain registrar: Namecheap
Hosting: Vercel (connected to GitHub)
