<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/atgora-forum/.github/main/assets/logo.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/atgora-forum/.github/main/assets/logo.svg">
  <img align="right" alt="ATgora Logo" src="https://raw.githubusercontent.com/atgora-forum/.github/main/assets/logo.svg" width="96">
</picture>

# atgora-website

**Marketing + documentation site for ATgora**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Next.js](https://img.shields.io/badge/Next.js-16-black)](https://nextjs.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Next.js](https://img.shields.io/badge/Next.js-16-black)](https://nextjs.org/)

---

## 🚧 Status: Planned (Q2 2026)

The marketing and documentation website at atgora.forum.

**Current phase:** Repository will be created in Phase 1

---

## What is this?

The atgora-website hosts:

**Marketing pages (`/`):**
- Homepage - Hero, key benefits, CTAs
- Features - What ATgora does
- Pricing - Managed hosting tiers
- Comparisons - vs Discourse, Flarum, Circle, etc.
- Blog - Technical posts, community stories
- About - Who, why, open source commitment

**Documentation (`/docs`):**
- Self-hosting guides
- Admin tutorials
- Plugin development
- Concepts (portable identity, cross-forum reputation)
- API integration guides

**Note:** API reference docs are served separately by atgora-api at `/docs` (auto-generated from code).

---

## Tech Stack

| Component | Technology |
|-----------|-----------|
| Framework | Next.js 16, React 19 |
| Styling | TailwindCSS, Radix Colors, Flexoki |
| Content | MDX (blog + docs) |
| SEO | JSON-LD, OpenGraph, sitemaps |
| Analytics | Plausible (privacy-focused, optional) |
| Deployment | Vercel or self-hosted |

---

## Pages Structure

```
/                    Homepage
/features            Feature overview
/pricing             Managed hosting tiers
/vs/discourse        Comparison pages
/vs/flarum
/vs/circle
/blog                Blog listing
/blog/[slug]         Blog posts (MDX)
/docs                Documentation home
/docs/[...slug]      Documentation pages (MDX)
/about               About ATgora
```

---

## Development

**Prerequisites:**
- Node.js 24 LTS
- pnpm

**Setup:**
```bash
git clone https://github.com/atgora-forum/atgora-website.git
cd atgora-website
pnpm install
```

**Run development server:**
```bash
pnpm dev
```

**Run tests:**
```bash
pnpm test
pnpm lint
pnpm typecheck
```

---

## Content

**Blog posts:** `content/blog/*.mdx`
**Documentation:** `content/docs/**/*.mdx`

Both support:
- Frontmatter metadata
- MDX components
- Syntax highlighting (Shiki + Flexoki)
- Table of contents

---

## SEO

**Requirements:**
- Server-side rendering (SSR)
- JSON-LD structured data
- OpenGraph + Twitter Cards
- Sitemap generation
- robots.txt
- Fast page loads (Lighthouse > 90)

---

## Deployment

**Production:** Deployed to atgora.forum

**Method:**
- Vercel (recommended) - auto-deploy on push to `main`
- Or self-hosted via Docker

---

## License

**MIT** - Marketing and docs should be freely usable.

---

## Related Repositories

- **[atgora-api](https://github.com/atgora-forum/atgora-api)** - API reference docs (served at /docs)
- **[Organization](https://github.com/atgora-forum)** - All repos

---

## Community

- 🌐 **Website:** [atgora.forum](https://atgora.forum)
- 💬 **Discussions:** [GitHub Discussions](https://github.com/orgs/atgora-forum/discussions)
- 🐛 **Issues:** [Report bugs](https://github.com/atgora-forum/atgora-website/issues)

---

© 2026 ATgora. Licensed under MIT.
