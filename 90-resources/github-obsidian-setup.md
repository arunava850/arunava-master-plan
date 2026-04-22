# GitHub + Obsidian Git setup guide

## What this gives you

- Your vault lives in Obsidian on your Mac (edit freely)
- Every change syncs automatically to a GitHub repo
- Claude can read any file via its raw GitHub URL
- Claude gives you updated markdown → you paste back → auto-syncs to GitHub
- Full version history of every change ever made

---

## Step 1 — Create the GitHub repo

1. Go to github.com → New repository
2. Name it: `arunava-master-plan`
3. Set to **Private** (your plan is yours — keep it private)
4. Don't initialise with README (you'll push existing files)
5. Click Create repository
6. Copy the repo URL — looks like:
   `https://github.com/YOUR-USERNAME/arunava-master-plan.git`

---

## Step 2 — Push your existing vault to GitHub

Open Terminal on your Mac and run:

```bash
cd ~/Documents/Obsidian/arunava-master-plan

git init
git add .
git commit -m "Initial vault — master plan"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/arunava-master-plan.git
git push -u origin main
```

Your vault is now on GitHub.

---

## Step 3 — Install Obsidian Git plugin

1. Open Obsidian
2. Settings → Community plugins → Turn off Safe mode
3. Browse community plugins → Search "Obsidian Git"
4. Install → Enable

### Configure Obsidian Git

Settings → Obsidian Git:

| Setting | Value |
|---|---|
| Auto pull interval | 10 minutes |
| Auto commit and push interval | 10 minutes |
| Commit message | `vault: auto-sync {{date}}` |
| Pull on startup | Enabled |

Now your vault auto-syncs to GitHub every 10 minutes without you doing anything.

### Manual sync shortcuts

| Action | Shortcut |
|---|---|
| Commit and push | Cmd + Shift + G (customisable) |
| Pull | Cmd + Shift + P (customisable) |

---

## Step 4 — Get raw GitHub URLs for your key files

These are the URLs Claude uses to fetch your latest files.

Format: `https://raw.githubusercontent.com/YOUR-USERNAME/arunava-master-plan/main/PATH-TO-FILE.md`

### Your key file URLs (fill in your username)

```
HOME:
https://raw.githubusercontent.com/YOUR-USERNAME/arunava-master-plan/main/HOME.md

SKILL:
https://raw.githubusercontent.com/YOUR-USERNAME/arunava-master-plan/main/skill/SKILL.md

Build log:
https://raw.githubusercontent.com/YOUR-USERNAME/arunava-master-plan/main/20-100-days/build-log.md

Build ideas:
https://raw.githubusercontent.com/YOUR-USERNAME/arunava-master-plan/main/20-100-days/build-ideas.md

LinkedIn posts:
https://raw.githubusercontent.com/YOUR-USERNAME/arunava-master-plan/main/10-identity/linkedin-posts.md

Cricket roadmap:
https://raw.githubusercontent.com/YOUR-USERNAME/arunava-master-plan/main/30-cricket-analytics/roadmap.md
```

**Save these URLs** — paste them into Claude at the start of any session.

---

## Step 5 — Update SKILL.md with your GitHub URLs

Once your repo is live, add your actual GitHub username to the SKILL.md file under a new section:

```markdown
## GitHub vault URLs
Repo: https://github.com/YOUR-USERNAME/arunava-master-plan
Raw base: https://raw.githubusercontent.com/YOUR-USERNAME/arunava-master-plan/main/

Key files to fetch each session:
- skill/SKILL.md
- HOME.md
- 20-100-days/build-log.md
```

---

## How a working session looks

### Starting a session
Tell Claude:
> "Fetch my vault — here are the URLs: [paste raw URLs for SKILL.md + HOME.md + build-log.md]"

Claude fetches the files, reads your current status, and picks up exactly where you left off.

### During the session
Work normally. Claude gives you updated markdown as needed.

### Ending a session
1. Copy updated markdown from Claude
2. Paste into the relevant file in Obsidian
3. Obsidian Git auto-pushes within 10 minutes
   (or press Cmd+Shift+G to push immediately)

---

## Troubleshooting

### Obsidian Git not pushing
- Check Terminal: `cd ~/Documents/Obsidian/arunava-master-plan && git status`
- Make sure you're authenticated: `git config --global user.email "you@email.com"`

### Authentication issues on Mac
Use GitHub's credential helper or create a Personal Access Token:
- GitHub → Settings → Developer Settings → Personal Access Tokens → Generate new token
- Use this token as your password when Git asks

### Conflicts (if editing on multiple devices)
Always pull before editing: Cmd+Shift+P in Obsidian before starting work.

---

## Optional — GitHub mobile app

Install the GitHub mobile app on your phone. You can view any vault file on the go — useful for reviewing your plan or reading a post draft without opening your laptop.
