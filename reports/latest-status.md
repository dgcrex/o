# Project Status Dashboard

**As of: 2026-07-05** · Regenerated on request (registry claims daily 17:34 EOD automation, but see Automation runs — it has not executed since baseline).

## Active projects

| Project | Where | Deadline | Status | Progress | Notes |
| --- | --- | --- | --- | --- | --- |
| Capital Flywheel Agent | Replit | none set | 🟢 Active | unknown | Still last updated 2026-07-02 — no change in 3 days |
| My Operations Team (KAN) | Jira | none set | 🟡 New | 0% | Still no real issues filed |
| Ops Automation Hub | GitHub dgcrex/o | rolling | 🟡 At risk | scaffolded | Repo itself is fine, but the automations it documents are not running — see below |
| Linear workspace | Linear | — | ⚪ Empty | — | Still 0 projects; only stock onboarding issues (MUH-1…4), unchanged |
| Notion workspace | Notion | — | ⚪ Empty | — | No content yet |

**No project currently has a deadline set anywhere** — unchanged since baseline. Deadline tracking
is still blocked on choosing a source of truth (Linear vs Jira vs Notion vs GitHub milestones).

## Awaiting user decision

1. **Choose source of truth for deadlines** — Linear vs Jira (KAN) vs Notion vs GitHub milestones — still open
2. **Semrush plan** — upgrade for MCP access, or drop the connector — still open
3. **WorkOS** — admin action to re-enable MCP (auth OK, MCP server disabled by an admin) — still open
4. **Durable scheduling** — recreate the four in-session automations as permanent scheduled routines before they expire ~2026-07-10 — **more urgent now**: evidence below suggests they've already stopped running, not just at future risk of expiring

## Automation runs

| Automation | Registered schedule | Last actual run | Next scheduled | Findings |
| --- | --- | --- | --- | --- |
| Weekly Integration Health Audit | Mon 08:11 | 2026-07-03 (baseline) | Mon 2026-07-06 08:11 | Not yet due; 3 connectors flagged at baseline (WorkOS, Semrush, Spotify) |
| Morning Ops Brief | daily 06:57 | never confirmed | daily 06:57 | Read-only, notify-only — can't confirm execution from repo state |
| Midday Pulse | weekdays 12:21 | never confirmed | weekdays 12:21 | Read-only, notify-only — can't confirm execution from repo state |
| EOD Status Dashboard | daily 17:34 | **2026-07-03** (2 days ago) | daily 17:34 | ⚠️ **Missed 07-04 and 07-05 runs** — this job commits+pushes on every run, and no commits landed between the baseline and this manual regeneration |

⚠️ **Automation health flag**: the registry's cron IDs (`a96d56e0`, `470c4406`, `0b82cece`, `3298a020`)
are session-scoped per `automations/registry.md`, and this session's cron list is empty — consistent
with the jobs having lapsed rather than merely being close to their ~7-day expiry. Recommend treating
task #4 above (durable scheduling) as time-sensitive rather than a background chore.
