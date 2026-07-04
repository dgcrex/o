# Project Status Dashboard

**As of: 2026-07-04** · Live sweep (Linear, Notion, Jira KAN, Replit, Google Calendar,
GitHub `dgcrex/o` re-checked directly; full 15-system audit not due until Monday).

## Active projects

| Project | Where | Deadline | Status | Progress | Notes |
| --- | --- | --- | --- | --- | --- |
| Capital Flywheel Agent | Replit | none set | 🟢 Active | unknown | Still the most active real project; **no update since 2026-07-02** (2 days idle) |
| My Operations Team (KAN) | Jira | none set | 🟡 New | 0% | Still only the 2 stock onboarding tasks (KAN-1, KAN-2), both To Do — no real work logged yet |
| Ops Automation Hub | GitHub dgcrex/o | rolling | 🟢 Active | scaffolded | 0 open PRs/issues; working tree clean; this report is today's regeneration |
| Linear workspace | Linear | — | ⚪ Empty | — | Still 0 projects; only stock onboarding issues (MUH-1…4), all To Do |
| Notion workspace | Notion | — | ⚪ Empty | — | Search for "project status" returns 0 results — still no content |
| Google Calendar | Calendar | — | ⚪ Empty | — | 0 events through 2026-07-18 |

**No project currently has a deadline set anywhere** — unchanged from baseline. Deadline
tracking is still blocked on choosing a source of truth (see below).

## Awaiting your decision

1. **Choose source of truth for deadlines** — Linear vs Jira (KAN) vs Notion vs GitHub milestones. Unresolved since 2026-07-03.
2. **Semrush plan** — upgrade for MCP access, or drop the connector. Unresolved.
3. **WorkOS** — needs an admin to re-enable the org's MCP server (currently degraded). Unresolved.
4. **Durable scheduling — now time-sensitive**: the four automations below are session-scoped
   and auto-expire ~2026-07-10 (**6 days away**). This session's `CronList` currently shows
   **zero scheduled jobs**, so they are not verifiably running right now. Recreate them as
   permanent scheduled routines in the Claude Code web UI before the expiry window closes.

## Automations set to auto-iterate

| Automation | Registry schedule | Last run | Next scheduled run | Recent findings / errors |
| --- | --- | --- | --- | --- |
| Morning Ops Brief | daily 06:57 (`57 6 * * *`) | not confirmed run today | daily 06:57 | Not visible in this session's `CronList` — verify still active |
| Midday Pulse | weekdays 12:21 (`21 12 * * 1-5`) | not confirmed run today | next weekday 12:21 | Not visible in this session's `CronList` — verify still active |
| EOD Project Status Dashboard | daily 17:34 (`34 17 * * *`) | this report (manual/triggered run, 2026-07-04) | daily 17:34 | Producing this file; not visible in `CronList` as a standing job in this session |
| Weekly Integration Health Audit | Mondays 08:11 (`11 8 * * 1`) | 2026-07-03 baseline | Monday 2026-07-06, 08:11 | Baseline found 3 connectors needing attention: WorkOS (degraded), Semrush (unavailable), Spotify (unavailable — expired token) |

**Note**: `CronList` returning empty is expected for jobs created in a prior session context,
but combined with the registry's own durability caveat, this is worth confirming directly
rather than assuming the jobs are still firing.

## Summary

- **On track**: GitHub repo (clean, 0 open items), Capital Flywheel Agent (still the one real
  project, though idle 2 days).
- **At risk**: Automation durability — 6 days until the session-scoped cron jobs expire, and
  their current active status can't be confirmed from this session.
- **Needs your attention**: 4 unresolved decisions above, the same as yesterday — none are new,
  but none have been closed out either. Source-of-truth choice (#1) is now the single blocker
  keeping every project without a deadline.
