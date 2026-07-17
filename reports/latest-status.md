# Project Status Dashboard

**As of: 2026-07-17** · Manual regeneration (no live cron — see Automation runs below). Live sweep of GitHub `dgcrex/o`, Linear, Jira, and Notion.

## Active projects

| Project | Where | Deadline | Status | Progress | Notes |
| --- | --- | --- | --- | --- | --- |
| DWP UC appeal response | Notion Calendar / DWP (ref …744338) | **2026-07-18 — tomorrow** | 🔴 At risk | unconfirmed | VERIFIED via HMCTS/DWP email 21/06. Not tracked as an issue anywhere with an owner; no confirmed action taken. |
| GMP/IOPC escalation (MUH-21, MUH-25) | Linear (Muhammad Ikram team) | SAR ref. ~13 Jul, itself flagged **unverified** from the original letter, already passed either way | 🔴 Stalled 12 days | 0/5 questions answered | P0. MUH-25 (finalize draft, held for L4/L5 approval) is blocked on this. |
| Personal-ops casework backlog | Linear (Obsidian Command import, 7/5) | none tracked besides above | 🔴 Stalled 12 days | 0/26 issues done | 8 P0/Urgent issues (MUH-5,6,7,8,9,20,21,24) untouched since import — all blocked purely on facts/decisions only Rex can supply. |
| Ops Automation Hub | GitHub `dgcrex/o` | rolling | 🟡 At risk | scaffolded, reports current | **6 open draft PRs** (#1–#6, opened 7/5→7/16) all proposing the same dashboard regen, none merged or closed. Zero live cron jobs. |
| Capital Flywheel Agent | Replit | none | 🟡 Stale/unknown | unknown | Last confirmed update 2026-07-02 (15 days ago); unreachable in recent sweeps (needs reauth per 7/11 run). |
| My Operations Team (KAN) | Jira | none | ⚪ Empty | 0% | Still just the 2 stock onboarding tasks (KAN-1, KAN-2); unchanged since baseline. |
| Linear workspace (as project container) | Linear | — | ⚪ No formal projects | — | 0 Linear "Projects" defined even though 26 real issues exist under one team. |
| Notion workspace | Notion | — | 🟢 Active (casework only) | — | Populated with Command Tower / casework pages; still 0 content matching generic "project" tracking. |

## Awaiting your approval or decision

1. **DWP UC appeal response — due tomorrow (2026-07-18)**, no confirmed owner action. Highest-priority item on the board.
2. **PR triage** — 6 open draft PRs on `dgcrex/o` (#1–#6) all propose the same dashboard-regeneration content; every one of them has itself recommended merging one and closing the rest. None acted on in 12 days.
3. **MUH-21** — answer the 5 GMP escalation questions (SAR deadline referenced inside is itself unverified — needs the original letter checked).
4. **7 more stalled P0/Urgent personal-ops issues** (MUH-5 police facts, MUH-6 safeguarding intake, MUH-7 send approved drafts, MUH-8 HMCTS case-number check, MUH-9 send landlord details, MUH-20 police report, MUH-24 welfare-rights advice) — all blocked purely on facts or one-tap actions only you can supply.
5. **Two unverified social-engineering flags**, carried forward unresolved since 7/8: a spoofed `no-reply-claude@mail.anthropic.com` email, and a Drive-access request from `muhammadrex245@gmail.com` claiming to be "Rex." Neither has been acted on — please verify independently rather than clicking through.
6. **Connector decisions** (baseline 7/3, never re-audited): WorkOS MCP disabled by an admin; Semrush needs a plan upgrade for MCP access; Spotify's OAuth status is unconfirmed since the token was reported expired.
7. **Durable scheduling** — all 4 automations below have been fully expired (0 live cron jobs) since ~2026-07-10. Recreate them as permanent scheduled routines in the Claude Code web UI, or accept manual-only regeneration going forward.

## Automation runs

| Automation | Registered schedule | Actually running? | Last effective run | Next run | Findings |
| --- | --- | --- | --- | --- | --- |
| Morning Ops Brief | daily 06:57 | ❌ no live cron job | none confirmed | — | Documentation only since ~7/10 expiry. |
| Midday Pulse | weekdays 12:21 | ❌ no live cron job | none confirmed | — | Documentation only since ~7/10 expiry. |
| EOD Project Status Dashboard | daily 17:34 | ❌ no live cron job; kept alive only by manual runs | manual run 2026-07-16 (PR #6) | this run, 2026-07-17 | DWP deadline moved from "2 days" to **tomorrow**; PR backlog grew to 6; personal-ops backlog now 12 days stalled with zero movement. |
| Weekly Integration Health Audit | Mondays 08:11 | ❌ no live cron job | 2026-07-03 baseline only | none scheduled | `reports/integration-health.md` is now **14 days stale**; WorkOS/Semrush/Spotify items from baseline never re-checked. |

`CronList` confirms zero scheduled jobs exist in this session, consistent with every sweep since 7/6.

## Summary

- **On track**: repo scaffold itself is fine; Jira KAN and the Linear "projects" layer are intentionally empty and need no action.
- **At risk**: Capital Flywheel Agent (15 days stale, unreachable); integration health snapshot (14 days stale, three unresolved connector issues); automation reliability (all 4 jobs dead for a week+, GitHub hygiene degrading — 6 unmerged PRs).
- **Needs immediate attention**: DWP appeal response due tomorrow; PR merge/close triage; MUH-21's 5 GMP questions; 7 more stalled P0 personal-ops issues; durable-scheduling decision.
