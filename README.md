# Arunava Master Plan — Vault README

> Quick reference for syncing this vault with Claude and GitHub.

---

## GitHub repository

```
https://github.com/arunava850/arunava-master-plan
```

**Raw file base URL:**
```
https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/
```

---

## Starting a Claude session

Paste this exact message at the start of any new Claude conversation:

```
Please read my vault and get up to speed. Here are the key files:

SKILL: https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/skill/SKILL.md
HOME: https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/HOME.md
BUILD LOG: https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/20-100-days/build-log.md
PRIORITIES: https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/00-overview/what-to-do-first.md
```

Claude will fetch all four files, read your current status, and pick up exactly where you left off.

---

## Fetching a specific file mid-session

If you need Claude to read a specific note during a session, paste:

```
Please fetch and read this vault file:
https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/[folder]/[filename].md
```

### Common file URLs

| File | URL |
|---|---|
| Home | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/HOME.md` |
| SKILL | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/skill/SKILL.md` |
| Big picture | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/00-overview/big-picture.md` |
| Flywheel | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/00-overview/flywheel.md` |
| Audiences | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/00-overview/audiences.md` |
| What to do first | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/00-overview/what-to-do-first.md` |
| Positioning | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/10-identity/positioning.md` |
| LinkedIn posts | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/10-identity/linkedin-posts.md` |
| 100 days overview | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/20-100-days/overview.md` |
| Build ideas | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/20-100-days/build-ideas.md` |
| Build log | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/20-100-days/build-log.md` |
| Cricket roadmap | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/30-cricket-analytics/roadmap.md` |
| Content engine | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/40-content-engine/system.md` |
| Revenue streams | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/50-revenue-streams/overview.md` |
| Artist service | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/50-revenue-streams/artist-service.md` |
| Website architecture | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/60-website/architecture.md` |
| Certifications | `https://raw.githubusercontent.com/arunava850/arunava-master-plan/main/70-certifications/path.md` |

---

## Ending a Claude session

At the end of every session ask Claude:

```
Please give me the updated vault files from this session so I can sync to GitHub.
```

Claude will generate updated markdown for every file that changed. You paste each one into Obsidian and Obsidian Git auto-pushes to GitHub.

---

## Asking Claude to update a specific file

```
Please update my vault file [filename] with [what changed] and give me the markdown to paste in.
```

Example:
```
Please update my build-log.md — I completed Day 1 today. I built an AI caption generator for artists using the Claude API. It took 3 hours. The surprising thing was how much better the captions were when I added the artist's style as context.
```

---

## Git commands (Terminal)

**Push changes manually** (if Obsidian Git doesn't auto-push):
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

**Force push if needed:**
```bash
git push --force
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
│   └── what-to-do-first.md
├── 10-identity/
│   ├── positioning.md
│   └── linkedin-posts.md
├── 20-100-days/
│   ├── overview.md
│   ├── build-ideas.md
│   └── build-log.md
├── 30-cricket-analytics/
│   └── roadmap.md
├── 40-content-engine/
│   └── system.md
├── 50-revenue-streams/
│   ├── overview.md
│   └── artist-service.md
├── 60-website/
│   └── architecture.md
├── 70-certifications/
│   └── path.md
├── 80-build-log/
│   └── index.md (create when needed)
└── 90-resources/
    └── github-obsidian-setup.md
```

---

## Where new content goes

| Content type | File to update |
|---|---|
| New LinkedIn post | `10-identity/linkedin-posts.md` |
| New build idea | `20-100-days/build-ideas.md` |
| Completed build | `20-100-days/build-log.md` |
| Cricket finding | `30-cricket-analytics/findings.md` |
| Priority change | `00-overview/what-to-do-first.md` |
| New revenue idea | `50-revenue-streams/overview.md` |
| Website change | `60-website/architecture.md` |
| Cert progress | `70-certifications/path.md` |
