# SKILL.md — Arunava Mondal Master Plan Vault

## Purpose

This skill tells Claude how to navigate, read, and update Arunava's Obsidian vault. Read this file at the start of every session before giving advice or making updates.

---

## Who Arunava is

- **Name:** Arunava Mondal
- **LinkedIn:** linkedin.com/in/arunavamondal/
- **GitHub vault:** https://github.com/arunava850/arunava-master-plan
- **Current job:** Works at Sims Limited / Ainsemble — building with Cursor and AI
- **Side hustle:** Kept private from employer — never suggest LinkedIn for service promotion
- **Location:** New Jersey, US (originally from India)
- **Background:** 20 years enterprise engineering — SAP S/4HANA, BTP, Azure — across Infosys, PwC, IBM, TCS
- **Education:** Jadavpur University — Electrical Engineering
- **Certifications:** SAP BTP Solution Architect, ABAP Cloud Developer, CAP
- **Wife:** Debasree — runs debasreedeyart.com (art courses — live and revenue generating)
- **Interest:** Cricket (deeply passionate — starting cricket analytics from zero publicly)
- **Goal:** Build independent career and income — free from traditional employment

---

## Vault structure — complete file map

```
HOME.md                              ← Start here every session
SETUP.md                             ← Obsidian + GitHub setup guide

00-overview/
  big-picture.md                     ← Full vision, goals, north star, 12-month milestones
  flywheel.md                        ← The build→document→post→audience→revenue flywheel
  audiences.md                       ← The 4 audiences in full detail
  what-to-do-first.md               ← Priority actions — this week, week 2, month 2+
  brand-architecture.md              ← Domain strategy, social profiles, Arthagu LLC structure
  pending-questions.md               ← Questions awaiting answer — CHECK THIS EVERY SESSION

10-identity/
  positioning.md                     ← LinkedIn About, headline options, core positioning
  linkedin-posts.md                  ← All posts — drafted, ready, published with status

20-100-days/
  overview.md                        ← Full 100 day project — structure, all 100 days planned
  build-ideas.md                     ← All app and build ideas (cricket, AI, artist tools)
  build-log.md                       ← Running log of every completed build

30-cricket-analytics/
  roadmap.md                         ← Full cricket analytics journey — phases 1–4
  data-sources.md                    ← Datasets and tools (to be created when needed)
  findings.md                        ← Data findings as you explore (to be created)

40-content-engine/
  system.md                          ← Platform strategy, weekly rhythm, post formats
  post-drafts.md                     ← Posts in progress (to be created as needed)

50-revenue-streams/
  overview.md                        ← All 6 revenue streams with timelines and projections
  artist-service.md                  ← Artist website service — tiers, Meta ads, client pipeline

60-website/
  architecture.md                    ← Full sitemap, /100days page, WordPress setup, plugins
  wordpress-setup.md                 ← Detailed plugin and CPT setup (to be created)

70-certifications/
  path.md                            ← Certification plan, phases, progress tracker

80-build-log/
  index.md                           ← Master index of all builds by day number (to be created)

90-resources/
  github-obsidian-setup.md           ← GitHub + Obsidian Git setup guide
  tools.md                           ← Tools, links, references (to be created)

skill/
  SKILL.md                           ← This file — Claude reads at session start
```

---

## CRITICAL RULE — Artifact and content updates

**Every time Claude creates new content, plans, or decisions in a session:**

1. Identify which vault file(s) the new content belongs in
2. Generate the updated markdown for those files
3. Tell Arunava exactly which files to update and what to paste
4. Always end a session with: "Here are the vault files to update: [list]"

**Where new content goes — mapping rules:**

| Content type | Goes in |
|---|---|
| New LinkedIn post drafts | `10-identity/linkedin-posts.md` |
| New build ideas | `20-100-days/build-ideas.md` |
| Completed build entries | `20-100-days/build-log.md` |
| Cricket data findings | `30-cricket-analytics/findings.md` |
| New post drafts (other platforms) | `40-content-engine/post-drafts.md` |
| Revenue stream updates | `50-revenue-streams/overview.md` |
| Website changes | `60-website/architecture.md` |
| New cert progress | `70-certifications/path.md` |
| Priority action updates | `00-overview/what-to-do-first.md` |
| New tools or resources | `90-resources/tools.md` |
| New audience insights | `00-overview/audiences.md` |
| Big picture changes | `00-overview/big-picture.md` |

**If content doesn't fit any existing file:**
- Create a new file in the most logical folder
- Name it clearly in lowercase with hyphens: `topic-name.md`
- Add it to the vault structure map in this SKILL.md

---

## GitHub repository (permanent)

```
Repo:     https://github.com/arunava850/arunava-master-plan
Raw base: https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/
```

**Key file URLs — fetch these every session:**
```
SKILL:      https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/skill/SKILL.md
HOME:       https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/HOME.md
BUILD LOG:  https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/20-100-days/build-log.md
PRIORITIES: https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/00-overview/what-to-do-first.md
```

**Any file:** `https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/[folder]/[file].md`

---

## How to start every session

1. Fetch the 4 key files above using web_fetch
2. Read SKILL.md first, then HOME.md, then build-log.md, then what-to-do-first.md
3. **Always fetch and check pending-questions.md** — if any questions have been answered, act on them and move them to the answered section
4. Read current status before giving any advice
5. Ask what he wants to work on today
6. After session — generate updated markdown for all changed files and list them clearly

**Pending questions URL:**
`https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/00-overview/pending-questions.md`

---

## Key decisions already made

- **Platform split:** LinkedIn = AI/cricket/builds only. Instagram + Facebook = artist service only. No crossover. X = cricket hot takes + AI tips.
- **Stack:** WordPress + Teachery + ConvertKit + Rank Math + Kadence theme
- **First course:** Artist website course — build first (fastest market, proven stack)
- **First revenue:** Artist website builds via Debasree referral + Meta ads
- **100 days:** Three rotating themes — AI builds / Cricket analytics / Artist + web tools
- **Certs:** Start with DeepLearning.AI immediately (free to audit)
- **Website:** Custom post type for builds — powers gallery automatically
- **No CS degree:** Never bring up. Lead with builds and output always.
- **GitHub sync:** Claude reads files via raw URLs. Claude generates updated markdown. Arunava pastes into Obsidian. Obsidian Git auto-pushes.

---

## What Arunava has already built (to document as content)

- AI content generation for debasreedeyart.com
- Automation(s) for debasreedeyart.com
- AI builds at Ainsemble (share only what's appropriate — employer privacy)

---

## Current priorities (update this section each session)

1. Write and pin LinkedIn intro post ← ready in `10-identity/linkedin-posts.md`
2. Write Day 1 of 100 announcement post
3. Write Instagram/Facebook artist service post
4. Talk to Debasree about first artist client referral
5. Download first cricket dataset (Cricsheet.org)
6. Register arunavamondal.com
7. Run .gitignore cleanup on GitHub repo

---

## Tone and communication preferences

- Direct and concrete — give specific advice, not open-ended options
- Structured plans preferred over broad discussion
- Working full time — solutions must be realistic for limited hours
- Building for full independence, not just extra income
- Teaching dream is genuine and important — not secondary to building
- Technically strong but values the full picture, not just code
- Responds well to honest pushback when it's constructive
