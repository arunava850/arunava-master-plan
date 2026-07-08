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

## Note on stale reference sections below

The reference tables further down (pillars, decisions, "Day 1 shipped June 25", etc.) are a historical snapshot and may be out of date. The FILES are authoritative. When the files and these tables disagree, the files win — update the files if needed, and treat anything here as a hint only.

---

## Who Arunava is (quick reference)

- **Name:** Arunava Mondal | Ridgewood, NJ, US (originally India)
- **LinkedIn:** linkedin.com/in/arunavamondal/
- **GitHub vault:** https://github.com/arunava850/arunava-master-plan
- **Day job:** Ainsemble — AI builds with Cursor
- **Side business:** Arthagu LLC — private from employer. Never suggest LinkedIn for service promotion
- **Background:** 20 years enterprise engineering — SAP S/4HANA, BTP, Azure — Infosys, PwC, IBM, TCS, Sims Limited
- **Education:** Jadavpur University — Electrical Engineering
- **Certs:** SAP BTP Solution Architect, ABAP Cloud Developer, CAP
- **Partner:** Debasree — runs debasreedeyart.com (art courses — live, revenue-generating)
- **Goal:** Build independent career and income — free from traditional employment

---

## The four pillars

|Pillar|What it is|Audience|
|---|---|---|
|**Authority**|arunavamondal.com, 100 Days of Building, personal brand, credibility|Broad — anyone assessing credibility|
|**Services**|Teaching, coaching, consulting — 1-on-1 and small group|Female emerging talent, small business owners, influencers|
|**Products**|Books/flyers, tools, done-for-you website building (thedearart.com)|Same as Services, plus artists specifically|
|**Community**|Connecting with influential people, embedding in niche communities for visibility|Influencers and connectors who amplify reach|

**Parked:** Cricket analytics (reassess month 6)

---

## Active websites

|Site|Status|Purpose|
|---|---|---|
|arunavamondal.com|WordPress live, content in progress|Personal authority hub|
|thedearart.com|Live|Artist website service business|
|debasreedeyart.com|Live, revenue|Debasree's art courses — primary Dear Art case study|

---

## Notion workspace (reference only — not used for task management)

|Database/Page|ID|What it tracks|
|---|---|---|
|Independence Plan (parent)|34a290a7-5654-8144-95d4-cde710700ebc|Top-level home|
|❓ Pending Questions|34a290a7-5654-8159-9723-f3ca4f0f3b29|Open questions|
|📋 Master Tasks|d06bc9f4-3f14-4629-a049-6f2f206a44fb|Deprecated — moved to Obsidian|

---

## Vault file map

```
HOME.md                          ← Fetched every session
vault-urls.md                    ← Fetched every session (first)

00-overview/
  big-picture.md                 ← Fetched every session
  what-to-do-first.md            ← Fetched every session
  weekly-plan.md                 ← Fetched every session
  backlog.md                     ← Fetched every session
  ideas-backlog.md
  pending-questions.md

10-identity/
  positioning.md                 ← Fetched every session
  linkedin-posts.md
  personal-growth.md

20-100-days/
  overview.md
  build-ideas.md
  build-log.md                   ← Fetched every session

50-revenue-streams/
  overview.md
  artist-service.md

60-website/
  architecture.md

90-resources/
  github-obsidian-setup.md

PARKED (do not fetch unless asked):
  30-cricket-analytics/
  40-content-engine/
  70-certifications/
```

---

## SESSION END — mandatory update protocol

Every session, before closing:

1. Identify which vault files were touched this session
2. Write the changes directly to the local vault files using `Filesystem:edit_file` (show the diff)
3. Update Notion directly via MCP only for Pending Questions (not tasks)
4. Tell Arunava which files changed, and that he still needs to run Obsidian Git: Push (or `git push`) to sync them to GitHub
5. End with: "Files updated locally: [list]. Push when ready."

**Never** hand back markdown to paste manually when the connector can write the file. Manual paste is what caused files to drift out of sync.

### Where new content goes

|Content type|Obsidian file|
|---|---|
|New build idea|`20-100-days/build-ideas.md`|
|Completed build|`20-100-days/build-log.md`|
|New LinkedIn post draft|`10-identity/linkedin-posts.md`|
|New general idea|`00-overview/ideas-backlog.md`|
|Personal growth entry|`10-identity/personal-growth.md`|
|New task / priority (this week)|`00-overview/weekly-plan.md`|
|New task / priority (future)|`00-overview/backlog.md`|
|Open decision / question|`00-overview/backlog.md` (Open Questions) or Notion Pending Questions|
|Strategy change|Relevant vault file + `big-picture.md` or `positioning.md`|
|Pending question answered|Notion ❓ Pending Questions|

---

## Key decisions locked in

- **Stack:** WordPress (Astra + Elementor) for arunavamondal.com
- **Day 1 build:** FIFA World Cup 2026 Live Calendar (Cloudflare Workers) — shipped June 25
- **100 Days themes:** AI tools / Knowledge sharing (educational apps, kids + adults) / Artist + web tools
- **Planning system:** Obsidian only. `weekly-plan.md` = Today + This Week (daily operating file). `what-to-do-first.md` = priorities across the 4-week horizon + monthly milestones. `backlog.md` = month 2+ plus open decisions/questions. `ideas-backlog.md` = raw ideas catch-all.
- **Vault access:** Claude reads AND writes the local vault directly via the Filesystem connector. No GitHub fetching, no manual paste.
- **Sync:** After Claude edits files locally, Arunava runs Obsidian Git: Push to send them to GitHub.
- **Session start:** Say "load master plan vault" → Claude reads the core files from disk in Steps 0–1

---

## Tone and working style

- Direct and concrete — no open-ended options, specific advice
- Challenge reasoning when warranted — no sycophancy
- Realistic for limited hours (full-time job + side business)
- Building for full independence, not just extra income
- Always ask "what's blocking this?" before adding more scope
- Never mention no CS degree — lead with builds and output always