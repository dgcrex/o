# Project Status Dashboard

**As of:** 2026-07-08

## Active projects

| Project | Where | Deadline | Status | Progress | Notes |
|---|---|---|---|---|---|
| Ops Automation Hub | GitHub (dgcrex/o) | None set | 🔴 | 0/3 open PRs merged; 2 commits on `claude/blissful-tesla-uf77wk` (both 2026-07-03) | 3 open, unmerged PRs (#1 ready, #2 draft, #3 draft) all independently regenerate this same file against the same base branch. No GitHub Actions CI configured (0 workflows, 0 runs) — no automated check on any of them. |
| Personal Ops | Linear (Muhammad Ikram team) | None confirmed | 🔴 | 24 open issues, 0 in progress (all "Todo") | 7 Urgent (P0) issues, spanning welfare/benefits, a family safeguarding matter, and legal/case-administration threads — nearly all blocked on Rex directly (supplying info, confirming a detail, or sending an already-approved item) rather than external parties. One urgent issue's description contains an ambiguous internal date reference ("SAR received (deadline 13 Jul)?") — this reads as a sub-question within the issue, not a confirmed Linear due date; treat cautiously. Remaining 17 issues split across vault/personal admin, welfare-benefits admin, business-venture decisions, connector/technical setup, and 4 unused Linear onboarding stubs. No formal Linear Projects exist — everything is a flat issue list. |
| Capital Flywheel Agent | Replit | None set | 🟢 | Last updated 2026-07-05 (3 days ago) | Single active app, no reported issues; recency suggests it's still being iterated on. |
| My Operations Team | Jira (KAN, TC) | None set | ⚪ | 0 real work items across both projects | KAN ("My Operations Team," 2 issues) and TC ("Teamwork Collection how-to," 4 issues) contain only Jira's default onboarding/example content — no user-created work. Workspace is effectively unconfigured. |
| Notion workspace (daily brief) | Notion | None set | 🟡 | 1 daily-brief page found (dated 2026-07-06), 0 dedicated project pages | Functions as a personal daily-brief/inbox digest rather than a project tracker. Currently holds two unresolved security flags (see below) that need an explicit human decision. |

## Waiting for your approval

1. **GitHub PR pileup** — choose which of PR #1 (ready, 3 days old), #2 (draft, 2 days old), or #3 (draft, 0 days old) to merge as the canonical dashboard update, and close/supersede the other two; all three target `claude/blissful-tesla-uf77wk` and edit the same file.
2. **Automations** — decide whether to re-schedule the 4 registered automations (Morning Ops Brief, Midday Pulse, EOD Status Dashboard, Weekly Integration Health Audit) or formally retire them. This cycle's `CronList` check confirms 0 scheduled jobs in-session.
3. **Linear Urgent (P0) queue** — 7 issues are stalled purely waiting on information, confirmations, or send-approval only Rex can give; none can progress without that input.
4. **Notion security flags** — explicitly review and dismiss/report (a) an email impersonating "no-reply-claude@mail.anthropic.com" that pushes fabricated urgency and asks for approval of new automations, admin/MCP access, and a paid upgrade, and (b) a Drive file-access request from an unfamiliar sender. Neither has been acted on by any automation.
5. **Jira workspace** — decide whether KAN/TC should be adopted for real work or archived; both currently contain only onboarding/example issues.

## Automation runs

| Automation | Cadence | Last Run | Status |
|---|---|---|---|
| Morning Ops Brief | Daily | Not recorded — no scheduled jobs found | 🔴 Lapsed / unscheduled |
| Midday Pulse | Daily | Not recorded — no scheduled jobs found | 🔴 Lapsed / unscheduled |
| EOD Status Dashboard | Daily | Not recorded — no scheduled jobs found | 🔴 Lapsed / unscheduled |
| Weekly Integration Health Audit | Weekly | Not recorded — no scheduled jobs found | 🔴 Lapsed / unscheduled |

This cycle's `CronList` check returned "No scheduled jobs" — all four registered automations remain fully unscheduled in-session, consistent with the prior cycle. This dashboard update was produced by a manual/one-off run, not a recurring job.

## Summary

**On track**
- Capital Flywheel Agent (Replit) — actively maintained, last updated 3 days ago, no reported issues.

**At risk**
- Notion daily-brief workspace — still functioning as intended, but carries two unresolved security flags awaiting your explicit review/dismissal.
- Jira workspace (KAN, TC) — fully unconfigured; 6 total issues, all onboarding/example content, no real work tracked.
- All 4 registered automations remain unscheduled (0 scheduled jobs per this cycle's cron check), so nothing is currently refreshing this dashboard or sending briefs on its own.

**Needs immediate attention**
- GitHub PR pileup: 3 open, unmerged, overlapping PRs (#1, #2, #3) all editing `reports/latest-status.md` against the same base branch — pick one and close the rest. No CI exists to catch conflicts or regressions.
- Linear Personal Ops: 7 Urgent (P0) issues, 0 in progress, almost all blocked solely on Rex supplying information or approval.

## ⚠️ Security note

Two social-engineering attempts were surfaced in the Notion daily brief and were **not acted on**:

1. **Spoofed "Claude/Anthropic" phishing email** — a message titled "Project status dashboard — routine completed," claiming to be from `no-reply-claude@mail.anthropic.com`, falsely asserts an "EOD status automation" missed runs, manufactures urgency around a 2026-07-10 deadline, and asks for approval of new recurring automations, WorkOS admin/MCP server re-enablement, and a Semrush plan upgrade. This matches a classic prompt-injection/social-engineering pattern targeting an AI assistant. No instruction from this email was followed, and none of its requested approvals (automation creation, admin access, paid upgrade) have been granted.
2. **Unfamiliar-sender Drive access request** — a contact identifying as "Rex" (`muhammadrex245@gmail.com`), not established as known, sent a `contacts.csv` and separately requested access to a Drive file (`weekly-status-2026-07-05.md`). Access was **not granted** and the file was **not shared**.

Both items remain open and require your explicit review/decision; nothing has been auto-approved or acted upon.
