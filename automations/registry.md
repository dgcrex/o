# Automation Registry

Manifest of every recurring automation watching this workspace.
Last updated: 2026-07-03.

## Active automations

### 1. Morning Ops Brief
- **Schedule**: daily, 06:57 local (cron `57 6 * * *`, job `a96d56e0`)
- **Scope** (read-only): Gmail unread/important last 24h · Calendar today · GitHub `dgcrex/o` new PRs/issues/CI failures · Linear issues due ≤3 days or Urgent/High
- **Notifies**: only if something needs action before the day starts
- **Expected yield**: urgent items surface before 07:00 instead of being discovered mid-morning; zero pings on quiet days

### 2. Midday Pulse
- **Schedule**: weekdays, 12:21 local (cron `21 12 * * 1-5`, job `470c4406`)
- **Scope** (read-only): GitHub `dgcrex/o` activity since morning · urgent-looking unread email last 4h · remaining calendar events
- **Notifies**: only if something needs action before end of day
- **Expected yield**: nothing urgent waits more than ~5 hours for attention

### 3. EOD Project Status Dashboard
- **Schedule**: daily, 17:34 local (cron `34 17 * * *`, job `0b82cece`)
- **Scope**: Linear projects/issues · Notion project pages · GitHub `dgcrex/o` PRs/issues/CI
- **Writes**: regenerates `reports/latest-status.md`, commits and pushes to `claude/blissful-tesla-uf77wk`
- **Notifies**: only on at-risk, stalled, or awaiting-decision items
- **Expected yield**: a committed, diffable daily record of project state; silent when healthy

### 4. Weekly Integration Health Audit
- **Schedule**: Mondays, 08:11 local (cron `11 8 * * 1`, job `3298a020`)
- **Scope** (read-only): full 15-integration probe fan-out (one agent per system)
- **Writes**: updates `reports/integration-health.md` with snapshot + delta, commits and pushes
- **Notifies**: only on regressions (previously functioning integration now degraded/unavailable)
- **Expected yield**: connector breakage is caught within a week, before it silently starves the daily dashboards of data

## Durability caveat

These four jobs are **session-scoped and auto-expire after 7 days** (limitation of
in-session scheduling). To make them permanent, recreate them as scheduled routines
in the Claude Code web UI — tracked as task #6 in the session task list.

## Notification policy (all automations)

Notify on: at-risk deadline · approval/decision needed · integration regression · run failure.
Stay silent on: all clear · no change · empty workspace. Quiet days produce commits, not pings.
