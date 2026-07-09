# Website architecture — arunavamondal.com

## Stack
- **CMS:** WordPress (same as debasreedeyart.com — don't reinvent)
- **Theme:** Kadence (free, fast, builder-friendly)
- **Courses:** Teachery — new school under existing account
- **Payments:** Teachery built-in Stripe (may not need WooCommerce)
- **Email:** ConvertKit (free to 10,000 subscribers)
- **SEO:** Rank Math
- **Cache:** WP Fastest Cache

---

## Full sitemap

| Page | URL | Purpose |
|---|---|---|
| Home | / | Hook + latest builds + newsletter CTA |
| Projects | /projects | Gallery of all builds — filterable. No day counter, no finish line. |
| Writing | /writing | Long-form articles and tutorials — SEO engine |
| Services | /services | Website builds (artists + creators) + coaching — activate when ready |
| Courses | /courses | Teachery course landing pages — add when first course ready |
| About | /about | Full story, credentials, the why |
| Newsletter | /newsletter | Simple sign-up — "build log" |

---

## The projects page (/projects)

### Header
- "Builds" — short intro line. NO day counter, NO progress bar, NO finish line. Builds accumulate as they ship.

### Filter bar
- All · AI Tools · Artist + Web · Automations · Data Visualisations
- (No cricket filter — parked.)

### Gallery grid
- Card per build: title + category tags + date
- Each card links to individual build page

---

## Individual build page structure (/projects/[slug])

1. **Header** — title, date, category badge, 2-line summary
2. **The build** — screenshot, GIF, or embedded demo (first thing people see)
3. **What I built** — 2–3 paragraphs, plain language
4. **How I built it** — tech stack, decisions, code snippets
5. **What surprised me** — most human and shareable section
6. **Links** — demo / GitHub / LinkedIn post
7. **Navigation** — ← previous build · next build →
8. **CTA at bottom** — newsletter (most builds) or Services (artist/creator builds)

---

## WordPress setup — key technical decisions

### Custom post type for builds (most important)
Use CPT UI plugin to create a "Build" custom post type with fields:
- Category
- Date shipped
- Demo URL
- GitHub URL
- LinkedIn post URL
- Build summary (2 lines)

This powers the entire /projects gallery automatically. Add a new entry per build — 10 minutes. No manual page editing ever. (No "day number" field — builds aren't numbered.)

---

## Required plugins (free to start)

| Plugin | Purpose |
|---|---|
| CPT UI | Creates "Build" custom post type |
| Advanced Custom Fields | Adds custom fields to each build |
| Kadence Blocks | Gallery grid and filter UI on /100days |
| ConvertKit for WordPress | Newsletter forms everywhere |
| Rank Math SEO | Auto-optimises every build page |
| WP Fastest Cache | Site speed |

**Rule:** No more than these 6 to start.

---

## Homepage sections (top to bottom)

1. **Hero** — one sentence + name + photo + "See what I'm building →" (→ /projects)
2. **Latest 3 builds** — auto-updates from custom post type
3. **What I do** — build useful things with AI · help artists & creators get online · teach and connect
4. **Newsletter sign-up** — "build log"
5. **About — short version** — 2–3 sentences + link to full About page

---

## Build order (minimum viable first)

- **Week 1:** Home + /projects gallery + About live (WordPress already installed; add Kadence + 6 plugins). Ship rough.
- **Week 2:** "Build" custom post type + add FIFA and the caption generator as the first entries
- **Week 3:** Refine /projects filters; About polished; ConvertKit newsletter live
- **Week 4:** Home copy reflects current positioning; Services page stub; Rank Math on all build pages
- **Ongoing:** Add one build entry per build — 10 minutes each

---

## SEO note

Every build page = one indexed article. Over time you'll accumulate dozens of pages working for you permanently. "How I built a live World Cup calendar on Cloudflare Workers" will rank on Google for years.
