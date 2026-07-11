# Project Status Dashboard

**As of: 2026-07-11** · Live sweep (GitHub, Linear, Jira, Notion, Superhuman Mail, WorkOS, GitHub Actions).
Gmail, Google Calendar, and Replit could not be checked this run — those connectors need
reauthorization before an automation can read them.

## Active projects

| Project | Where | Deadline | Status | Progress | Notes |
| --- | --- | --- | --- | --- | --- |
| Personal Ops (Rex / "Obsidian Command") | Linear, team "Muhammad Ikram" | **13 Jul** (SAR + welfare-advice items) | 🔴 At risk | 0/20 (0%) | 20 issues imported 2026-07-05 from an Obsidian vault; every issue is Todo/Backlog and blocked on Rex's own input — 7 are P0/Urgent |
| Ops Automation Hub | GitHub `dgcrex/o` | rolling | 🟡 At risk | scaffolded | Repo itself is fine, but 3 near-duplicate "regenerate dashboard" PRs (#1, #2, #3) have sat open/unmerged since Jul 5–8 |
| Capital Flywheel Agent | Replit | none set | ⚪ Unverified | unknown | Replit connector needs reauth this session; last confirmed activity was 2026-07-05 |
| My Operations Team (KAN) | Jira | none set | 🟡 Stale | 0% | Still only the 2 stock onboarding tasks; no real work items filed since baseline |
| Notion workspace | Notion | — | 🟢 Active | — | Daily "Obsidian Command — Tray" briefs are running (Jul 8, Jul 9 entries found) and are the most current record of inbox/calendar chores |

No project has a deadline set in a project-management tool itself — the only concrete date
(13 Jul) lives inside Linear issue text (SAR + welfare-rights items), not a due-date field.

## Awaiting your decision

1. **Merge or close GitHub PRs #1, #2, #3** — all three propose the same dashboard regeneration and are still open/unmerged (oldest since 2026-07-05). Recommend picking one (or this update) and closing the rest.
2. **7 P0/Urgent Linear issues, all blocked on facts only Rex holds** (MUH-5, 6, 7, 8, 9, 20, 21, 24, 25 span P0/P1) — none are actionable by an assistant per their own approval gates. **MUH-21 references a 13 Jul SAR deadline — 2 days away.**
3. **WorkOS** — `whoami` now reports "No WorkOS dashboard account backs this login"; needs `setup_account` or an admin action.
4. **Semrush** — plan still lacks MCP access; decide upgrade vs. drop.
5. **Durable scheduling** — `CronList` confirms 0 jobs are currently scheduled anywhere live. The 4 automations described in `automations/registry.md` are documentation only right now, not running jobs.

## Security — verify yourself, nothing below was acted on

- **Phishing / prompt-injection attempt**: an email impersonating Claude/Anthropic (`no-reply-claude@mail.anthropic.com`) closely mirrors this dashboard's own language ("4 decisions await you," durable scheduling, WorkOS, Semrush) to manufacture urgency. Surfaced via the Jul 8 Notion brief; not clicked, not acted on.
- **Drive access request**: an email from "Rex" at `muhammadrex245@gmail.com` (not your own `dgcrex@gmail.com`) asked to access `weekly-status-2026-07-05.md` and separately sent a `contacts.csv`. Note your own Jira/Linear identity is also displayed as "Rex" (`dgcrex@gmail.com`) — worth confirming this second address is someone you actually recognize before sharing anything.

## Automation runs

| Automation | Last confirmed run | Registered schedule | Findings |
| --- | --- | --- | --- |
| 15-system health sweep | 2026-07-03 (baseline; not re-run this session) | Mon 08:11 weekly | Baseline flagged WorkOS, Semrush, Spotify — all three still unresolved |
| Morning Ops Brief | unconfirmed (read-only, no commit trail) | daily 06:57 | — |
| Midday Pulse | unconfirmed (read-only, no commit trail) | weekdays 12:21 | — |
| EOD Status Dashboard | this update (manual) | daily 17:34 | Underlying repo trunk (`claude/blissful-tesla-uf77wk`) hasn't been updated since baseline — PRs #1–#3 never merged |

`CronList` returned zero scheduled jobs this session — in-session cron does not persist
across sessions, so durable scheduling (a permanent routine in the Claude Code web UI) is
still the only fix, per `automations/registry.md`.
