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
| Home | / | Hook + live 100 days counter + 3 latest builds + newsletter CTA |
| 100 Days | /100days | Gallery of all builds — filterable, with progress bar |
| Cricket analytics | /cricket | All cricket builds and findings — standalone for shareability |
| Writing | /writing | Long-form articles and tutorials — SEO engine |
| Services | /services | Artist website builds + AI consulting — for Instagram/Facebook traffic only |
| Courses | /courses | Teachery course landing pages — add when first course ready |
| About | /about | Full story, credentials, the why |
| Newsletter | /newsletter | Simple sign-up — "weekly build log" |

---

## The 100 days page (/100days)

### Header (always visible)
- Live progress: "Day 47 of 100 · 47 builds shipped"
- Progress bar (updates automatically)
- Start date and end date

### Filter bar
- All · AI Tools · Cricket Analytics · Artist + Web · Automations · Data Visualisations
- Week 1 · Week 2 · Week 3 ... (sequential reading)

### Gallery grid
- Card per build: day number + title + category tags
- Each card links to individual build page

---

## Individual build page structure (/100days/day-47)

1. **Header** — day number, title, date, category badge, 2-line summary
2. **The build** — screenshot, GIF, or embedded demo (first thing people see)
3. **What I built** — 2–3 paragraphs, plain language
4. **How I built it** — tech stack, decisions, code snippets
5. **What surprised me** — most human and shareable section
6. **Links** — demo / GitHub / LinkedIn post / YouTube video
7. **Navigation** — ← previous build · next build →
8. **CTA at bottom** — newsletter (cricket builds) or services (artist builds)

---

## WordPress setup — key technical decisions

### Custom post type for builds (most important)
Use CPT UI plugin to create a "Build" custom post type with fields:
- Day number
- Category
- Demo URL
- GitHub URL
- LinkedIn post URL
- YouTube video URL
- Build summary (2 lines)

This powers the entire gallery automatically. Add a new entry per build — 10 minutes. No manual page editing ever.

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

1. **Hero** — one sentence + name + photo + "Follow the 100 day project →"
2. **Live 100 days counter** — "Day 47 of 100 — currently building: [title]"
3. **Latest 3 builds** — auto-updates from custom post type
4. **Three pillars** — AI builds · Cricket analytics · Helping artists get online
5. **Newsletter sign-up** — "Weekly build log"
6. **About — short version** — 2–3 sentences + link to full About page

---

## Build order (minimum viable first)

- **Week 1:** Register domain + WordPress install + Kadence + holding page (2 hours)
- **Week 2:** Set up Build custom post type + add first 3 past builds
- **Week 3:** Build /100days gallery page with filters and progress bar
- **Week 4:** Homepage + About + Services page + ConvertKit + Rank Math
- **Ongoing:** Add one build entry per build — 10 minutes each

---

## SEO note

Every build page = one indexed article. After 100 days you'll have 100 pages working for you permanently. "How I built a T20 win probability model" will rank on Google for years.
