# Arunava Master Plan — Vault Loader

You've triggered the master plan vault loader. Follow ALL steps in order. Do not skip any step.

**Source of truth: the local vault on disk. Never fetch from GitHub raw URLs — they lag, rate-limit, and have failed in practice. Always read files with the Filesystem connector.**

**Vault root:**
```
/Users/arunavamondal/Documents/Business/Career/git-claude/arunava-master-plan/
```

---

## STEP 0 — Confirm connector access

Call `Filesystem:list_allowed_directories`. The vault root above must be inside an allowed directory. If it is not, stop and tell Arunava the Filesystem connector needs to be enabled/scoped for that folder — do not fall back to GitHub fetching, and do not reconstruct vault contents from memory.

---

## STEP 1 — Read the core vault files

Read ALL of these in one `Filesystem:read_multiple_files` call. Paths are relative to the vault root above.

```
HOME.md
vault-urls.md
00-overview/big-picture.md
00-overview/weekly-plan.md
00-overview/what-to-do-first.md
00-overview/backlog.md
00-overview/ideas-backlog.md
10-identity/positioning.md
20-100-days/build-log.md
```

If a file read fails, say so explicitly. Do not invent, guess, or paper over its contents from memory. A missing file is reported as missing.

For any other file needed later in the session, get its path from `vault-urls.md`'s file list (use the file names, read locally — ignore the raw URLs in that file).

---

## STEP 2 — State the current state from what you just READ

Do NOT recite a hardcoded anchor. Read the actual current state out of the files and report it, including:

- Latest entry in `build-log.md` (which Day, shipped or not, published or not)
- Today + This Week from `weekly-plan.md` (the daily operating file)
- This week's non-negotiables from `what-to-do-first.md`
- Any open decisions/questions in `backlog.md`
- The four pillars and audience exactly as written in `HOME.md` / `positioning.md`

**If files contradict each other** (e.g. build-log shows a build shipped but HOME.md still says "Day 0 not started"), flag the contradiction explicitly and ask which is correct before proceeding. Do not silently pick one.

---

## STEP 3 — Surface priorities and ask

Surface:

- **Today + This Week** from `weekly-plan.md` (this is the daily operating file — lead with it)
- This week's non-negotiables from `what-to-do-first.md`
- Anything unfinished or unpublished from `build-log.md` (an unshipped/unpublished build is the top priority per the decision rules)
- Open decisions from `backlog.md` that are blocking work

Then ask what Arunava wants to work on.

---

## Note on the reference sections below

The quick-reference below is CONTEXT, not truth. Anything about current status (which Day, what's shipped, what's this week) MUST come from reading the files in Step 1 — never from this section and never from memory. If this section and a file disagree, the file wins.

**Hard rule learned the hard way:** never state a fact about the vault's contents, a file's existence, or current status without having just read it or listed it this session. If you haven't verified it this session, say "let me check" and run the read/list first. Do not infer a file's absence from another file's index — list the directory. Do not describe file contents from memory — read the file.

---

## Who Arunava is (stable background — rarely changes)

- **Name:** Arunava Mondal | Ridgewood, NJ, US (originally India)
- **LinkedIn:** linkedin.com/in/arunavamondal/
- **GitHub vault:** https://github.com/arunava850/arunava-master-plan
- **Local vault root:** `/Users/arunavamondal/Documents/Business/Career/git-claude/arunava-master-plan/`
- **Day job:** Ainsemble — AI builds with Cursor
- **Side business:** Arthagu LLC — umbrella for everything. PRIVATE from employer. Never suggest LinkedIn for service promotion.
- **Background:** 20 years enterprise engineering — SAP S/4HANA, BTP, Azure — Infosys, PwC, IBM, TCS, Sims Limited
- **Education:** Jadavpur University — Electrical Engineering
- **Certs:** SAP BTP Solution Architect, ABAP Cloud Developer, CAP
- **Partner:** Debasree — runs debasreedeyart.com (art courses — live, revenue-generating). Primary Dear Art proof point.
- **Goal:** Build independent career and income — free from traditional employment
- **Never mention:** no CS degree. Lead with builds and output.

---

## Actual vault file map (verified 2026-07-08 by full directory read)

Read every session (Step 1):
```
HOME.md
vault-urls.md
00-overview/big-picture.md      ← UPDATED file, most current strategy
00-overview/weekly-plan.md      ← daily operating file (Today + This Week)
00-overview/what-to-do-first.md
00-overview/backlog.md          ← month 2+ AND open decisions (Q12–Q14)
00-overview/ideas-backlog.md
10-identity/positioning.md      ← UPDATED file, current identity
20-100-days/build-log.md
```

Read on demand (get exact names from the tree, do not guess):
```
00-overview/audiences.md          00-overview/brand-architecture.md
00-overview/flywheel.md           00-overview/pending-questions.md
10-identity/linkedin-posts.md     10-identity/personal-growth.md
20-100-days/overview.md           20-100-days/build-ideas.md
50-revenue-streams/overview.md    50-revenue-streams/artist-service.md
60-website/architecture.md        90-resources/github-obsidian-setup.md
README.md   SETUP.md   VAULT-UPDATE-COMPLETE.md
```

Parked (do not read unless asked):
```
30-cricket-analytics/roadmap.md
40-content-engine/content-ideas.md   40-content-engine/system.md
70-certifications/path.md
```

**Known vault issues to be aware of (verified 2026-07-08 — recheck, may be fixed):**
- The strategy pivoted in July (four pillars = Authority/Services/Products/Community; audience = emerging female talent + female small business owners; cricket parked). `big-picture.md`, `positioning.md`, `backlog.md` reflect this. But `HOME.md`, `weekly-plan.md`, `what-to-do-first.md`, `overview.md`, and `audiences.md` still describe the OLD plan (Day 1 = "AI caption generator", cricket as active audience, June-10 framing). When these disagree, the July-dated files win. Offer to reconcile the stale ones.
- `build-log.md` shows Day 1 = FIFA World Cup 2026 Live Calendar, built + deployed (wc2026-calendar.arthagu.workers.dev) but NOT yet published (no LinkedIn post; link is `[to be filled]`). `HOME.md`/`weekly-plan.md` still say "Day 0 / start caption generator." Confirm actual status with Arunava rather than trusting either in isolation.
- `README.md` and `SETUP.md` describe an old Notion-based, GitHub-fetch workflow. Superseded: planning is Obsidian-only, access is local connector.
- There is a junk directory literally named `{00-overview,10-identity,...}` at the vault root (a mis-fired shell brace-expansion). Empty. Flag for deletion; don't write into it.
- `vault-urls.md` lists raw GitHub URLs — use it only for the list of filenames, read those files locally. Do not fetch the URLs.

---

## Notion (reference only — NOT the task system; Obsidian is)

| Page | ID | Use |
|---|---|---|
| Independence Plan (parent) | 34a290a7-5654-8144-95d4-cde710700ebc | Top-level home |
| ❓ Pending Questions | 34a290a7-5654-8159-9723-f3ca4f0f3b29 | Only thing still updated in Notion |
| 📋 Master Tasks | d06bc9f4-3f14-4629-a049-6f2f206a44fb | DEPRECATED — moved to Obsidian |

---

## SESSION END — mandatory update protocol

Before closing every session:

1. Identify which vault files were touched this session.
2. Write changes DIRECTLY to the local files using `Filesystem:edit_file`, and show the diff. Never hand back markdown to paste by hand — manual paste is what let files drift out of sync.
3. Before asserting anything about a file while editing, re-read it — do not edit from memory of what it "probably" contains.
4. Update Notion via MCP only for Pending Questions.
5. Tell Arunava exactly which files changed and that he still needs to run Obsidian Git: Push (or `git push`) to sync to GitHub — the connector writes local files, it does not push.
6. End with: "Files updated locally: [list]. Push when ready."

### Where new content goes

|Content type|File|
|---|---|
|New build idea|`20-100-days/build-ideas.md`|
|Completed build|`20-100-days/build-log.md`|
|New LinkedIn post draft|`10-identity/linkedin-posts.md`|
|New general idea|`00-overview/ideas-backlog.md`|
|Personal growth entry|`10-identity/personal-growth.md`|
|Task/priority (this week)|`00-overview/weekly-plan.md`|
|Task/priority (future)|`00-overview/backlog.md`|
|Open decision/question|`00-overview/backlog.md` (Open Questions) or Notion Pending Questions|
|Strategy change|Relevant file + `big-picture.md` and/or `positioning.md`|

---

## Tone and working style

- Direct and concrete — specific advice, not open-ended option menus
- Challenge reasoning when warranted — no sycophancy
- Verify before asserting — the failure mode to avoid is confident claims about vault state that turn out wrong
- Realistic for limited hours (full-time job + side business)
- Always ask "what's blocking this?" before adding scope
- Never mention no CS degree — lead with builds and output