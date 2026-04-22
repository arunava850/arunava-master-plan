# Setup instructions

## Getting this vault into Obsidian on Mac

### Step 1 — Move the folder
After downloading, move the `arunava-master-plan` folder to:
```
~/Documents/Obsidian/arunava-master-plan/
```

### Step 2 — Open as a vault in Obsidian
1. Open Obsidian
2. Click "Open another vault" (bottom left)
3. Select "Open folder as vault"
4. Navigate to `~/Documents/Obsidian/arunava-master-plan/`
5. Click Open

### Step 3 — Recommended Obsidian settings
- Enable **Graph view** (left sidebar) — shows how all notes connect
- Enable **Backlinks** panel — shows which notes link to each note
- Install the **Dataview** plugin (community plugins) — lets you build dynamic tables from your build log
- Install the **Calendar** plugin — visual weekly view of your build activity

### Step 4 — Set HOME.md as your default startup note
Settings → Options → Files & Links → Default new tab behaviour → Set to HOME.md

---

## Using this vault with Claude

Every time you start a new Claude conversation in this project:
1. Reference the vault by saying "check the vault" or "update the vault"
2. Claude will read SKILL.md first to get up to speed
3. After the session, ask Claude to "update the vault with what we decided today"

The vault grows with you. Add new builds, new post drafts, new ideas, new progress — it becomes your living business operating system.

---

## Folder structure explained

```
arunava-master-plan/
├── HOME.md                    ← Open this first every time
├── skill/
│   └── SKILL.md               ← Claude reads this to understand your context
├── 00-overview/               ← The big picture and goals
├── 10-identity/               ← LinkedIn, positioning, posts
├── 20-100-days/               ← The 100 day project
├── 30-cricket-analytics/      ← Cricket journey
├── 40-content-engine/         ← Content system and rhythm
├── 50-revenue-streams/        ← All revenue paths
├── 60-website/                ← arunavamondal.com build plan
├── 70-certifications/         ← Cert plan and progress
├── 80-build-log/              ← Master build index
└── 90-resources/              ← Tools, links, references
```

---

## Adding a new build (takes 5 minutes)

1. Open `20-100-days/build-log.md`
2. Copy the template at the top
3. Fill in: day number, title, what you built, what surprised you, links
4. Save
5. Open `80-build-log/index.md` and add one line entry

That's it. The website pulls from WordPress — this vault is your personal record.
