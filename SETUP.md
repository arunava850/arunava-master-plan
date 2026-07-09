# Setup instructions

## This vault

Lives at:
```
/Users/arunavamondal/Documents/Business/Career/git-claude/arunava-master-plan/
```
Open this folder as a vault in Obsidian. It's a git repo — Obsidian Git handles sync to GitHub (arunava850/arunava-master-plan).

---

## Recommended Obsidian settings

- **Graph view** + **Backlinks** — see how notes connect
- **Obsidian Git** plugin — auto-commit + push (this is what syncs to GitHub)
- Set `HOME.md` as the default startup note (Settings → Files & Links → Default new tab)

---

## Using this vault with Claude

1. Start a session by saying **"load master plan vault"** — Claude reads the core files directly from disk via the Filesystem connector (no GitHub fetching, no pasting URLs).
2. Work.
3. Claude writes any changes **directly to the local files** and shows diffs.
4. **You then push:** run Obsidian Git: Push (or `git push`). The connector writes locally — it does NOT push for you.

The vault is your living operating system — it grows as you build.

---

## Current folder structure

```
arunava-master-plan/
├── HOME.md                    ← Open first
├── skill/SKILL.md             ← Claude's session loader (also copied into Claude Settings → Skills)
├── 00-overview/               ← big-picture, weekly-plan, what-to-do-first, backlog, audiences, etc.
├── 10-identity/               ← positioning, linkedin-posts, personal-growth
├── 20-100-days/               ← build-log + build-ideas (the "100 days" name is retired; just builds now)
├── 30-cricket-analytics/      ← PARKED
├── 40-content-engine/         ← content system (older reference)
├── 50-revenue-streams/        ← revenue overview + Dear Art artist-service
├── 60-website/                ← arunavamondal.com architecture
├── 70-certifications/         ← cert plan (backlog)
└── 90-resources/              ← tools, setup
```

---

## Adding a new build

1. Open `20-100-days/build-log.md`, copy the template, fill in title, date, what you built, what surprised you, links. (No day numbers — builds aren't numbered.)
2. Add the build to arunavamondal.com via the "Build" custom post type → it appears on /projects automatically.
3. Publish the LinkedIn post; paste its URL back into the build-log entry and the CPT.
