# Project Status Dashboard

**As of: 2026-07-12** · Manual regeneration (the scheduled 17:34 EOD automation has not
run since baseline — `CronList` confirms zero jobs currently scheduled anywhere).
Live sweep of GitHub `dgcrex/o`, Linear, and Notion.

## Active projects

| Project | Where | Deadline | Status | Progress | Notes |
| --- | --- | --- | --- | --- | --- |
| GMP/SAR legal escalation | Linear (Rex personal-ops) | **2026-07-13 (tomorrow)** | 🔴 At risk | blocked | MUH-21 (P0): 5 escalation questions incl. "SAR received (deadline 13 Jul)?" — unanswered, blocked entirely on Rex |
| UC appeal (DWP, ref …744338) | Notion Calendar | 2026-07-18 | 🟡 Upcoming | — | DWP response due; verified against HMCTS/DWP email 21/06/2026 |
| Rex personal-ops backlog | Linear (team "Muhammad Ikram") | mixed, mostly none set | 🔴 At risk | 0/29 (0%) | Imported 2026-07-05 from Obsidian vault; unchanged for 7 days; 9 P0/Urgent, 7 P1/High — every issue blocked on Rex input, evidence, or approval |
| Ops Automation Hub | GitHub `dgcrex/o` | rolling | 🟡 At risk | scaffolded, PR backlog | Repo itself fine; 4 open draft PRs (#1–#4, opened 7/5 → 7/11) all propose the same dashboard-regen content, none merged or closed |
| Capital Flywheel Agent | Replit | none set | ⚪ Unconfirmed | unknown | Not reachable this sweep (no Replit check performed today) |
| My Operations Team (KAN) | Jira | none set | ⚪ Unconfirmed | 0% | Not reachable this sweep |
| Notion workspace | Notion | — | 🟢 Active (content, not projects) | — | Populated with Obsidian Command vault pages, held-drafts calendar entries; still 0 items in a dedicated "Projects" database |

## Awaiting user decision

1. **Triage the 4 duplicate open PRs** (#1 7/5, #2 7/6, #3 7/8, #4 7/11 — all draft, all unmerged, all base `claude/blissful-tesla-uf77wk`, none of which targets `main`). Recommend: merge the most current (#4) and close #1–#3, or merge this update and close all four. Left as-is, every future run will keep adding a new one.
2. **SAR deadline 2026-07-13 (tomorrow)** — MUH-21 needs Rex's 5 answers before the escalation draft (MUH-25) can be finalized. This is the most time-sensitive item in the workspace right now.
3. **Two unresolved social-engineering flags** (carried forward unchanged from PRs #3 and #4, still sitting in the Notion-visible inbox as of this sweep):
   - An email spoofing `no-reply-claude@mail.anthropic.com` that mimics this dashboard's own language ("routine completed," project status, automations stopped). Anthropic does not send dashboard emails from that address — treat as phishing, do not click through.
   - An email from a "Rex" at `muhammadrex245@gmail.com` (not the account owner's `dgcrex@gmail.com`) requesting Google Drive access to a status file. Do not grant access without independently verifying the sender out-of-band.
4. **Choose a source of truth for deadlines** — Linear vs Jira (KAN) vs Notion vs GitHub milestones — still unresolved since baseline.
5. **WorkOS / Semrush connector decisions** — unresolved since baseline (WorkOS MCP disabled by admin; Semrush plan lacks MCP access).
6. **Durable scheduling** — recreate the four automations in `automations/registry.md` as permanent scheduled routines; the in-session versions have been fully lapsed since ~2026-07-05, not merely approaching expiry.

## Automation runs

| Automation | Last confirmed run | Next scheduled | Findings / errors |
| --- | --- | --- | --- |
| EOD Status Dashboard | 2026-07-03 (baseline); manual regenerations since via PRs on 7/5, 7/6, 7/8, 7/11, and this one on 7/12 | daily 17:34 (not actually scheduled — `CronList` returns 0 jobs) | Automation itself has not executed on its own since baseline; every update since has been a manual/ad hoc session |
| Weekly Integration Health Audit | 2026-07-03 (baseline only) | Mondays 08:11 (not actually scheduled) | Missed 7/6 and will miss 7/13 unless recreated; `reports/integration-health.md` is now 9 days stale |
| Morning Ops Brief | never confirmed run | daily 06:57 (not actually scheduled) | Read-only, no artifact to check |
| Midday Pulse | never confirmed run | weekdays 12:21 (not actually scheduled) | Read-only, no artifact to check |

**Bottom line on automations**: all four jobs listed in `automations/registry.md` are documentation only. No cron job has existed in any of the last five sessions that checked (`CronList` → empty every time). Recreating them as durable scheduled routines in the Claude Code web UI remains the single highest-leverage fix.
