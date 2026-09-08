# CLAUDE.md

Project notes for Claude Code sessions working in this repo. See `PRODUCT.md` for full brand/product context (audience, voice, design principles) — read that first for anything copy- or design-related.

## Blog

- Live at `blog/index.html` (listing) with individual posts as static HTML files under `blog/`, matching the rest of the site (no CMS, no build tooling anywhere in this repo).
- First post published: `blog/five-things-that-kill-a-local-business-website.html` — **"Five Things That Kill a Local Business Website."**
  - Picked deliberately: it doubles as SEO content (people search phrases like this) and as a soft pitch for outreach — it speaks directly to the bar/restaurant/local-business-owner audience described in `PRODUCT.md`, without being a sales pitch.
- "Blog" is in the main nav (header + footer where applicable) on every page, between Services and Résumé.
- Keep future posts in the site's established voice: bold, honest, direct — "the work is the argument," no filler, no generic agency-speak (see `PRODUCT.md` → Brand Personality / Design Principles / Anti-references).
- Post pages use `BlogPosting` JSON-LD (author/publisher reference the existing `#person` entity from `index.html`'s schema) — add the same block to future posts.
- To add a new post: create `blog/<slug>.html` (copy the existing post as a template), add a `post-card` entry to `blog/index.html`.
