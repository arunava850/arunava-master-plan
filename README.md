# Arunava Master Plan — Vault README

> Quick reference for syncing this vault with Claude and GitHub.

---

## GitHub repository

```
https://github.com/arunava850/arunava-master-plan
```

**Raw file base URL:**
```
https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/
```

---

## The two-system rule

> **Obsidian = thinking, writing, reference**
> **Notion = tracking, doing, managing**

When in doubt: would you want to filter it by status or date? → Notion. Are you writing or thinking? → Obsidian.

---

## What lives where

### Stays in Obsidian permanently
| File | What it is |
|---|---|
| `skill/SKILL.md` | Claude reads this every session — stays here always |
| `00-overview/big-picture.md` | Full vision, goals, north star |
| `00-overview/flywheel.md` | How everything connects |
| `00-overview/audiences.md` | The 4 audiences in detail |
| `00-overview/brand-architecture.md` | Domain strategy, social profiles |
| `10-identity/positioning.md` | LinkedIn About, headline, core positioning |
| `10-identity/linkedin-posts.md` | Post drafts and writing — text lives here |
| `20-100-days/overview.md` | 100 days structure and full plan |
| `20-100-days/build-ideas.md` | All scattered app/build ideas |
| `30-cricket-analytics/roadmap.md` | Cricket analytics journey plan |
| `30-cricket-analytics/findings.md` | Data findings and notebook-style thinking |
| `40-content-engine/system.md` | Platform strategy and weekly rhythm |
| `50-revenue-streams/overview.md` | Revenue stream strategy |
| `50-revenue-streams/artist-service.md` | Artist service strategy |
| `60-website/architecture.md` | Website sitemap and build plan |
| `70-certifications/path.md` | Certification plan |
| `90-resources/` | Tools, links, setup guides |

### Lives in Notion (not Obsidian)
| What | Notion database |
|---|---|
| Task tracking and status | 📋 Master Tasks |
| Each completed build entry | 🔨 100 Days Build Log |
| Post status (scheduled/published) | 📅 Content Calendar |
| Client and sales pipeline | 💰 Revenue Tracker |
| LinkedIn followers, email list, revenue numbers | 📊 KPI Dashboard |
| Pending questions awaiting answers | ❓ Pending Questions |

### Exists in both (different purpose)
| Content | In Obsidian | In Notion |
|---|---|---|
| LinkedIn posts | Full text draft | Status only (Idea/Ready/Published) + post URL |
| Build log | Longer reflection and learnings | Day number, category, links, summary |
| Priorities | Narrative "what to do first" reference | Live task list with status and phase |
| Pending questions | Strategy context around the question | The question + your answer field |

---

## What to update in Notion as you progress

### After completing a build
- Add entry to **🔨 100 Days Build Log** — day number, category, what you built, demo URL, LinkedIn post URL
- Mark the related task **Done** in **📋 Master Tasks**

### After publishing a post
- Update status to **Published** in **📅 Content Calendar**
- Add the live post URL to the Post URL field

### After getting a client or making a sale
- Add entry to **💰 Revenue Tracker** — client name, type, amount, source, status

### Every Monday morning (5 minutes)
- Update numbers in **📊 KPI Dashboard** — LinkedIn followers, email list, YouTube subscribers, revenue

### When you answer a pending question
- Update your answer in **❓ Pending Questions** in Notion
- Tell Claude: "I've answered some pending questions — please read the Notion page and continue"

### When a task phase changes or new tasks emerge
- Update **📋 Master Tasks** — change status, add new tasks, mark done

---

## Notion workspace

**Home page:** https://www.notion.so/34a290a75654814495d4cde710700ebc

---

## Starting a Claude session

Paste this at the start of any new Claude conversation:

```
Please read my vault and get up to speed. Here are the key files:

SKILL: https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/skill/SKILL.md
HOME: https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/HOME.md
BUILD LOG: https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/20-100-days/build-log.md
PRIORITIES: https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/00-overview/what-to-do-first.md
```

Claude will fetch all four files, read your current status, and pick up exactly where you left off.

---

## Fetching a specific file mid-session

```
Please fetch and read this vault file:
https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/[folder]/[filename].md
```

### Common file URLs

| File | URL |
|---|---|
| Home | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/HOME.md` |
| SKILL | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/skill/SKILL.md` |
| Big picture | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/00-overview/big-picture.md` |
| Flywheel | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/00-overview/flywheel.md` |
| Audiences | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/00-overview/audiences.md` |
| Brand architecture | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/00-overview/brand-architecture.md` |
| Positioning | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/10-identity/positioning.md` |
| LinkedIn posts | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/10-identity/linkedin-posts.md` |
| 100 days overview | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/20-100-days/overview.md` |
| Build ideas | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/20-100-days/build-ideas.md` |
| Build log | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/20-100-days/build-log.md` |
| Cricket roadmap | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/30-cricket-analytics/roadmap.md` |
| Content engine | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/40-content-engine/system.md` |
| Revenue streams | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/50-revenue-streams/overview.md` |
| Artist service | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/50-revenue-streams/artist-service.md` |
| Website architecture | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/60-website/architecture.md` |
| Certifications | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/refs/heads/main/70-certifications/path.md` |

---

## Ending a Claude session

At the end of every session ask Claude:

```
Please give me the updated vault files from this session so I can sync to GitHub.
```

Claude will generate updated markdown for every file that changed. You paste into Obsidian and Obsidian Git auto-pushes to GitHub.

---

## Asking Claude to update a specific file

```
Please update my vault file [filename] with [what changed] and give me the markdown to paste in.
```

Example:
```
Please update my build-log.md — I completed Day 1 today. I built an AI caption generator
for artists using the Claude API. It took 3 hours. The surprising thing was how much better
the captions were when I added the artist's style as context.
```

---

## Git commands (Terminal)

**Push changes manually:**
```bash
cd /Users/arunavamondal/Documents/Business/Career/git-claude/arunava-master-plan
git add .
git commit -m "update: [what you changed]"
git push
```

**Pull latest from GitHub:**
```bash
git pull
```

**Check what's changed:**
```bash
git status
```

**See recent commits:**
```bash
git log --oneline -10
```

---

## Obsidian Git shortcuts

| Action | How |
|---|---|
| Manual commit + push | Cmd + P → "Obsidian Git: Commit and sync" |
| Manual pull | Cmd + P → "Obsidian Git: Pull" |
| View git history | Cmd + P → "Obsidian Git: Open source control view" |

Auto-sync runs every 10 minutes when Obsidian is open.

---

## Vault folder structure

```
arunava-master-plan/
├── README.md                        ← You are here
├── HOME.md                          ← Open this first in Obsidian
├── SETUP.md                         ← GitHub + Obsidian Git setup guide
├── skill/
│   └── SKILL.md                     ← Claude reads this every session
├── 00-overview/
│   ├── big-picture.md
│   ├── flywheel.md
│   ├── audiences.md
│   ├── brand-architecture.md
│   ├── what-to-do-first.md          ← Narrative reference (live tasks in Notion)
│   └── pending-questions.md         ← Strategy context (live answers in Notion)
├── 10-identity/
│   ├── positioning.md
│   └── linkedin-posts.md            ← Post TEXT lives here (status in Notion)
├── 20-100-days/
│   ├── overview.md
│   ├── build-ideas.md
│   └── build-log.md                 ← Longer reflections (summary entries in Notion)
├── 30-cricket-analytics/
│   ├── roadmap.md
│   └── findings.md                  ← Create when you start exploring data
├── 40-content-engine/
│   └── system.md
├── 50-revenue-streams/
│   ├── overview.md
│   └── artist-service.md
├── 60-website/
│   └── architecture.md
├── 70-certifications/
│   └── path.md
└── 90-resources/
    ├── github-obsidian-setup.md
    └── tools.md                     ← Create when needed
```

---

## Where new content goes

| Content type | Goes in |
|---|---|
| New LinkedIn post draft | `10-identity/linkedin-posts.md` + status in Notion Content Calendar |
| New build idea | `20-100-days/build-ideas.md` |
| Completed build (full reflection) | `20-100-days/build-log.md` |
| Completed build (summary entry) | Notion 🔨 100 Days Build Log |
| Cricket data finding | `30-cricket-analytics/findings.md` |
| Post published | Update status + URL in Notion 📅 Content Calendar |
| New client or sale | Notion 💰 Revenue Tracker |
| Weekly metrics | Notion 📊 KPI Dashboard |
| Pending question answered | Notion ❓ Pending Questions |
| Strategy change | Relevant Obsidian note |
| New task or priority | Notion 📋 Master Tasks |
