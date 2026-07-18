# Project Status Dashboard

**As of: 2026-07-18** · Regenerated from a live sweep of GitHub `dgcrex/o`, Linear, Notion (incl. Notion Calendar), and session `CronList` state. Jira and Replit were not re-probed this run; their rows carry forward the last confirmed values.

## Active projects

| Project | Where | Deadline | Status | Progress | Notes |
| --- | --- | --- | --- | --- | --- |
| Ops Automation Hub | GitHub `dgcrex/o` | rolling | 🔴 At risk | scaffolded | **8 open draft PRs (#1–#8)** now propose the same dashboard-regeneration content, none merged since #1 (2026-07-05). Zero live automations. |
| Personal-ops backlog ("Obsidian Command") | Linear, team *Muhammad Ikram* | see below | 🔴 At risk | 0/26 done | Imported 2026-07-05, **13 days with zero completions**. 8 P0/Urgent issues, all blocked purely on facts/decisions only Rex can supply. |
| Obsidian Command / Command Tower | Notion | see below | 🟡 Active, blocked | partial | Substantial casework tracking (Critical Deadlines list, GMP/IOPC, PIP claim, Command Tower hub) but several dates still provisional/unverified; 12 held Gmail drafts awaiting a YES/NO review that was due 2026-07-08 (10 days overdue). |
| Capital Flywheel Agent | Replit | none set | 🟡 Stale (unverified) | unknown | Last confirmed update 2026-07-02; not re-probed this run. |
| My Operations Team (KAN) | Jira | none set | 🟡 New | 0% | Not re-probed this run; last known: no real issues filed. |

## ⚠️ Most time-sensitive item

**DWP UC appeal response (ref …744338) is due TODAY, 2026-07-18** — VERIFIED via HMCTS/DWP email ("Your UC appeal: appeal lodged"). No confirmed owner action found in Linear, Notion, or GitHub. This has been flagged as approaching in PRs #5, #6, and #7; it is no longer "coming up," it is due now.

Separately: Notion's "GMP / IOPC Complaint" page now states the SAR deadline was *"verified from source letter and met; complaint refs progressed."* This appears to contradict Linear issue **MUH-21** (P0, "Answer 5 GMP escalation questions"), which is still open/unanswered and references an unverified 13 Jul SAR deadline. Worth reconciling — either MUH-21 is stale and can be updated, or the Notion "met" note is premature.

## Awaiting your approval or input

1. **PR triage (now #1–#8)** — merge whichever has the freshest data and close the rest. Every sweep since 7/5 has flagged this and none has been resolved; the pile grows by one on every run of this dashboard task.
2. **DWP UC appeal response** — due today; needs a status check and, if unsent, immediate action.
3. **MUH-21 (P0)** — the 5 GMP escalation questions (any GMP reply since 16 Jun? recording ref? outcome letter? solicitor engaged? SAR received?) — blocks MUH-25 (draft finalization, held for L4/L5 approval).
4. **MUH-6 (P0)** — little-brother safeguarding intake — blocked purely on facts only Rex holds.
5. **MUH-5 (P0)** — return 9 police facts + same/separate-track decision — blocks MUH-20 (master police report, held for solicitor).
6. **MUH-24 (P0)** — book welfare-rights advice before fixing any enrolment date (protects UC entitlement) — do not fix an enrolment date first.
7. **MUH-8 (P0)** — confirm correct HMCTS case number (15 vs 16 digit mismatch found).
8. **MUH-9 (P0)** — send HOST landlord details (details held by Rex).
9. **MUH-7 (P0)** — already-approved SFE/GP/Salford/Study Tech drafts just need Rex's one-tap send.
10. **12 held Gmail drafts** ("Obsidian Command/HELD — Awaiting YES-NO") — review was due 2026-07-08, now 10 days overdue.
11. **Two unverified security flags (carried forward, unresolved)** — a spoofed `no-reply-claude@mail.anthropic.com` email, and a Google Drive access request from `muhammadrex245@gmail.com` claiming to be "Rex" (not the account owner's own `dgcrex@gmail.com`). Neither has been independently verified or acted on.
12. **Money decisions**: Slack Pro trial ends 2026-07-31 (keep/cancel); Atlassian Teamwork Premium trial ends 2026-08-02 (keep/cancel).
13. **Durable scheduling / WorkOS / Semrush / Spotify / deadline source-of-truth** — carried forward from baseline (2026-07-03), still undecided.

## Automations set to auto-iterate

| Automation | Last actual run | Next scheduled | Findings / errors |
| --- | --- | --- | --- |
| This status-dashboard task | today, 2026-07-18 (this run) | per its own external schedule (not session cron) | Confirms it runs as a durable scheduled routine, separate from the four session-cron jobs below. |
| Morning Ops Brief | never confirmed executed | none — session cron expired ~2026-07-10 | dead |
| Midday Pulse | never confirmed executed | none — session cron expired ~2026-07-10 | dead |
| Weekly Integration Health Audit | 2026-07-03 baseline only; missed its 2026-07-06 run | none — session cron expired ~2026-07-10 | `reports/integration-health.md` is now 15 days stale |

`CronList` confirms **zero** jobs currently scheduled in-session — the four automations documented in `automations/registry.md` remain dead, unchanged since roughly 2026-07-10. Only this dashboard task itself appears to run on a durable, non-session schedule.

## Summary

- **On track**: nothing currently — every workstream above has an overdue, blocked, or unresolved item.
- **At risk**: Ops Automation Hub (8-PR pileup, zero merges), Personal-ops backlog (13 days, 0/26 done, 8 P0s stalled).
- **Needs immediate attention**: DWP UC appeal response due **today**; the PR triage decision; MUH-21's 5 GMP questions; the 10-days-overdue held-draft review; the two unverified security flags.
