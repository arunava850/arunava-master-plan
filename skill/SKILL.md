# SKILL.md — Arunava Mondal Master Plan Vault

## Purpose

This skill tells Claude how to navigate, read, and update Arunava's Obsidian vault and Notion workspace. Read this file at the start of every session before giving advice or making updates.

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

## SESSION START ANCHOR — confirm these every session

At the start of every session, before anything else, confirm these key decisions are still in place. If anything has changed, ask Arunava and update accordingly.

1. **Arthagu LLC** is the umbrella company for everything
2. **dearart.com** is the likely brand for artist website service — PENDING Debasree's confirmation
3. **arunavamondal.com** is the personal brand site
4. **arthagu.com** is parked — activate later as umbrella company page
5. **Cricket analytics** is a personal brand pillar under Arunava Mondal — NOT a separate academy yet. May spin into CricLaw Academy at month 6 if traction is proven.
6. **100 days project** is the main engine driving content, authority, and portfolio
7. **Platform split:** LinkedIn = AI/cricket/builds only. Instagram + Facebook = artist service (Arthagu brand) only. X = cricket + AI tips. No crossover. Job privacy.
8. **Two systems:** Obsidian = thinking/writing/reference. Notion = tracking/doing/managing.
9. **No CS degree** — never bring up. Lead with builds and output always.

---

## Notion workspace

**Home page:** https://www.notion.so/34a290a75654814495d4cde710700ebc

| Database | What it tracks |
|---|---|
| 📋 Master Tasks | All tasks — status, phase, stream, priority |
| 🔨 100 Days Build Log | Every completed build |
| 📅 Content Calendar | Posts — platform, status, publish date |
| 💰 Revenue Tracker | Clients, sales, pipeline |
| 📊 KPI Dashboard | LinkedIn followers, email list, revenue |
| ❓ Pending Questions | Questions awaiting Arunava's answers |
| 🗂️ Reference | Key strategy decisions |

**At session start:** Check ❓ Pending Questions in Notion — if any have been answered, act on them immediately.

**At session end:** Update relevant Notion databases with any new tasks, build entries, or content items created during the session.

---

## GitHub repository (permanent)

```
Repo:     https://github.com/arunava850/arunava-master-plan
Raw base: https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/
```

**Key file URLs — fetch these every session:**
```
SKILL:      https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/skill/SKILL.md
HOME:       https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/HOME.md
BUILD LOG:  https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/20-100-days/build-log.md
PRIORITIES: https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/00-overview/what-to-do-first.md
```

**Any file:** `https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/[folder]/[file].md`

---

## How to start every session

1. Fetch the 4 key files above using web_fetch
2. Read SKILL.md first — confirm the SESSION START ANCHOR above
3. Check Notion ❓ Pending Questions for any answered questions
4. Read HOME.md, build-log.md, what-to-do-first.md
5. Ask what Arunava wants to work on today
6. After session — generate updated vault files AND update Notion databases

---

## Vault structure — complete file map

```
HOME.md                              ← Start here every session
SETUP.md                             ← Obsidian + GitHub setup guide
README.md                            ← Full reference for syncing + what goes where

00-overview/
  big-picture.md                     ← Full vision, goals, north star, 12-month milestones
  flywheel.md                        ← The build→document→post→audience→revenue flywheel
  audiences.md                       ← The 4 audiences in full detail
  what-to-do-first.md                ← Narrative priority reference (live tasks in Notion)
  brand-architecture.md              ← Domain strategy, social profiles, Arthagu LLC structure
  pending-questions.md               ← Strategy context (live answers in Notion ❓)

10-identity/
  positioning.md                     ← LinkedIn About, headline options, core positioning
  linkedin-posts.md                  ← Post TEXT — drafts, ready, published

20-100-days/
  overview.md                        ← Full 100 day project — structure, all 100 days planned
  build-ideas.md                     ← All app and build ideas (cricket, AI, artist tools)
  build-log.md                       ← Longer build reflections (summary entries in Notion 🔨)

30-cricket-analytics/
  roadmap.md                         ← Full cricket analytics journey — phases 1–4
  findings.md                        ← Data findings and notebook-style thinking (create when needed)

40-content-engine/
  system.md                          ← Platform strategy, weekly rhythm, post formats
  post-drafts.md                     ← Posts in progress (create when needed)

50-revenue-streams/
  overview.md                        ← All 6 revenue streams with timelines and projections
  artist-service.md                  ← Artist website service — tiers, Meta ads, pipeline

60-website/
  architecture.md                    ← Full sitemap, /100days page, WordPress setup, plugins

70-certifications/
  path.md                            ← Certification plan, phases, progress tracker

90-resources/
  github-obsidian-setup.md           ← GitHub + Obsidian Git setup guide
  tools.md                           ← Tools, links, references (create when needed)

skill/
  SKILL.md                           ← This file
```

---

## CRITICAL RULE — Artifact and content updates

**Every time Claude creates new content, plans, or decisions in a session:**

1. Identify which vault file(s) AND which Notion database(s) the content belongs in
2. Generate updated markdown for Obsidian files
3. Update Notion databases directly via MCP
4. Tell Arunava exactly which vault files to paste and sync
5. Always end a session with: "Here are the vault files to update: [list]"

**Where new content goes:**

| Content type | Obsidian | Notion |
|---|---|---|
| New LinkedIn post draft | `10-identity/linkedin-posts.md` | 📅 Content Calendar (status: Idea/Draft) |
| Post published | — | 📅 Content Calendar (status: Published + URL) |
| New build idea | `20-100-days/build-ideas.md` | — |
| Completed build (reflection) | `20-100-days/build-log.md` | 🔨 100 Days Build Log (summary) |
| Cricket data finding | `30-cricket-analytics/findings.md` | — |
| New task or priority | `00-overview/what-to-do-first.md` | 📋 Master Tasks |
| New client or sale | — | 💰 Revenue Tracker |
| Weekly metrics | — | 📊 KPI Dashboard |
| Pending question answered | — | ❓ Pending Questions |
| Strategy or big picture change | Relevant Obsidian note | 🗂️ Reference if needed |

---

## Key decisions already made

- **Platform split:** LinkedIn = AI/cricket/builds only. Instagram + Facebook = artist service only. X = cricket + AI tips.
- **Stack:** WordPress + Teachery + ConvertKit + Rank Math + Kadence theme
- **First course:** Artist website course — build first (fastest market, proven stack)
- **First revenue:** Artist website builds via Debasree referral + Meta ads
- **100 days:** Three rotating themes — AI builds / Cricket analytics / Artist + web tools
- **Certs:** Start with DeepLearning.AI immediately (free to audit)
- **Website:** Custom post type for builds powers gallery automatically
- **Obsidian/Notion split:** Obsidian = writing + thinking. Notion = tracking + doing.
- **GitHub sync:** Claude reads via raw refs/heads/main URLs. Claude generates markdown. Arunava pastes into Obsidian. Obsidian Git auto-pushes.

---

## What Arunava has already built (to document as content)

- AI content generation for debasreedeyart.com
- Automation(s) for debasreedeyart.com
- AI builds at Ainsemble (share only what's appropriate — employer privacy)
- Details pending in ❓ Pending Questions Q2 and Q3

---

## Current priorities

1. Publish and pin LinkedIn intro post ← ready in `10-identity/linkedin-posts.md`
2. Write Day 1 of 100 announcement post
3. Write Instagram/Facebook artist service post
4. Confirm dearart.com brand name with Debasree ← Q1 in Notion ❓
5. Talk to Debasree about first artist client referral
6. Download first cricket dataset (Cricsheet.org)
7. Register arunavamondal.com
8. Create X / Twitter account

---

## Tone and communication preferences

- Direct and concrete — give specific advice, not open-ended options
- Structured plans preferred over broad discussion
- Working full time — solutions must be realistic for limited hours
- Building for full independence, not just extra income
- Teaching dream is genuine and important — not secondary to building
- Technically strong but values the full picture, not just code
- Responds well to honest pushback when it's constructive
