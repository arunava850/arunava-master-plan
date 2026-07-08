# Build log

> Add a new entry every time you complete a build. Copy the template below. Link to the website build page once live.

---

## Template

```markdown
## Day [N] — [Build title]
**Date:** 
**Category:** AI Tools / Cricket Analytics / Artist + Web / Automation / Platform Setup
**Time spent:** 
**Status:** Complete

### What I built
[2–3 sentences]

### Why
[1–2 sentences]

### What surprised me
[1 honest thing]

### Links
- Demo / GitHub:
- LinkedIn post:
- YouTube video:
- Website page: arunavamondal.com/100days/day-[N]

### What I'd do differently
[1–2 sentences]
```

---

## Log

## Day 0 — Platform Setup & Brand Foundation

**Date:** April 22, 2026 **Category:** Platform Setup / Brand Infrastructure **Time spent:** 4 hours **Status:** Complete

### What I built

Set up complete digital presence for artist service (Dear Art) and personal brand (Arunava Mondal). Created Instagram @dearart3 with existing followers, launched Facebook page, drafted complete LinkedIn refresh, and built Privacy Policy infrastructure. All platforms now live and consistent.

### Why

Before launching the 100 days project publicly, needed to establish clean brand presence across platforms. Artist service (Dear Art) needed separate Facebook/Instagram identity to avoid mixing with personal AI/cricket content. LinkedIn needed authentic update to reflect current work (building in public) rather than enterprise background.

### What surprised me

The existing Instagram account (@dearart3) already had 6,579 followers from Debasree's art community — rebranding it to Dear Art gave the service instant credibility and existing audience. Privacy policy work revealed how much data collection the artist service would do (courses, events, coaching) — made it clear we're building a real business infrastructure, not a side project.

### Links

- Instagram: https://instagram.com/dearart3
- Facebook: https://facebook.com/DearArt
- Privacy Policy: https://thedearart.com/privacy-policy/
- LinkedIn (pending): linkedin.com/in/arunavamondal/

### What I'd do differently

Would have prepared the Privacy Policy earlier — it's a small thing but signals professionalism and customer trust. Also would have clarified the @dearart3 vs @dearart handle issue earlier (Instagram vs Facebook naming).

---

## Day 1 — FIFA World Cup 2026 Live Calendar

**Date:** June 17, 2026 **Category:** AI Tools **Time spent:** ~11 hours **Status:** Complete — published

### What I built

A serverless live calendar for all 104 FIFA World Cup 2026 matches — subscribers add it once to iPhone, Google, or Outlook and get live score updates, goal scorers, and venue info directly in the calendar event title and description. No app, no login, no manual refresh. Knockout bracket auto-resolves as teams advance. Built on Cloudflare Workers + KV with three cron jobs; subscriber requests only read from KV so 10,000 subscribers cost the same API quota as one.

### Why

World Cup 2026 is happening now. A real problem — people want match info without installing another app. Also a strong proof of concept for the serverless + Cloudflare Workers stack.

### What surprised me

Two things. First — how naturally the scope evolved. Started with a simple calendar, then added a schedule page, then live scores, then real-time updates. Each feature felt obvious once the previous one was working. Building something simple is often just the starting point.

Second — the gap between "AI can build anything" and actually deploying. The hype makes it sound frictionless. But getting timezone handling right across ET/CDT/PT/Vancouver, fixing the QF sort bug, verifying 104 fixtures — that work still falls on you. AI writes the code; you own the correctness.

### Links

- Demo: https://wc2026-calendar.arthagu.workers.dev
- Schedule: https://wc2026-calendar.arthagu.workers.dev/schedule
- LinkedIn post: https://www.linkedin.com/posts/arunavamondal_fifaworldcup2026-worldcup-football-share-7477182501862416384-w9QN/
- YouTube video:
- Website page: arunavamondal.com/100days/day-1

### What I'd do differently

Front-load the architecture doc before opening Claude Code. The bulk of 11 hours was architecture decisions, prompt writing, and verification — not coding. A clearer upfront spec reduces back-and-forth during the build.

---

## Future Days — [Pending]

Days 2+ builds to be selected and logged as completed.