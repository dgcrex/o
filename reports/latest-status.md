# Project Status Dashboard

**As of: 2026-07-06** · Manually regenerated (the automated daily 17:34 EOD job has not run since baseline — see automation status below). Supersedes the 2026-07-05 update proposed in open PR #1.

## Active projects

| Project | Where | Deadline | Status | Progress | Notes |
| --- | --- | --- | --- | --- | --- |
| Capital Flywheel Agent | Replit | none set | 🟢 Active | unknown | Updated 2026-07-05 (fresh) — still the most active real project in the workspace |
| My Operations Team (KAN) | Jira | none set | 🟡 New | 0% | Still no real issues filed since baseline |
| Ops Automation Hub | GitHub dgcrex/o | rolling | 🟡 At risk | scaffolded | Repo itself is fine, but every automation described in `automations/registry.md` has stopped running (see below) |
| Linear workspace | Linear | — | ⚪ Empty | — | Unchanged: 0 projects, only stock onboarding issues (MUH-1…4) |
| Notion workspace | Notion | — | ⚪ Empty | — | Unchanged: no content found |

**No project currently has a deadline set anywhere** — deadline tracking is blocked on choosing a source of truth (see below).

## Awaiting your approval / decision

1. **PR #1 open, unmerged** ("Update status dashboard: automation failures and stale project data") — opened 2026-07-05, still open a day later. Needs a merge/close decision; this update supersedes its content. → https://github.com/dgcrex/o/pull/1
2. **Choose source of truth for deadlines** — Linear vs Jira (KAN) vs Notion vs GitHub milestones. Nothing tracks a real deadline until this is picked.
3. **Semrush plan** — upgrade for MCP access, or drop the connector.
4. **WorkOS** — an admin must re-enable the disabled MCP server.
5. **Durable scheduling** — the four automations below are no longer running in-session at all; recreate them as permanent scheduled routines (Claude Code web UI) if you still want them.

## Automation status — action needed

All four automations in `automations/registry.md` were session-scoped and have now lapsed: `CronList` returns **zero** scheduled jobs, versus the four job IDs (`a96d56e0`, `470c4406`, `0b82cece`, `3298a020`) the registry documents as active. None of them ran on 2026-07-04, 05, or 06 — this dashboard update and PR #1 were both produced by manual/ad-hoc runs, not the scheduled jobs.

| Automation | Registered schedule | Last actual run | Next scheduled | Recent findings |
| --- | --- | --- | --- | --- |
| Morning Ops Brief | daily 06:57 | never (job gone) | none — not registered | — |
| Midday Pulse | weekdays 12:21 | never (job gone) | none — not registered | — |
| EOD Status Dashboard | daily 17:34 | never (job gone) | none — not registered | this file is being updated manually instead |
| Weekly Integration Health Audit | Mon 08:11 | 2026-07-03 (baseline only) | none — not registered | last real data: 3 connectors need attention (WorkOS, Semrush, Spotify) |

**Bottom line: none of the four automations are currently scheduled anywhere.** If durable scheduling isn't set up, this workspace is getting zero automatic monitoring right now.
