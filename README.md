# Ops Automation Hub

This repository is the durable home for automated operations reporting: recurring
status dashboards, integration health audits, and the manifest of every automation
that watches this workspace.

## Layout

| Path | Purpose |
| --- | --- |
| `automations/registry.md` | Manifest of every recurring automation: schedule, scope, notification policy, expected yield |
| `reports/latest-status.md` | Most recent end-of-day project status dashboard (regenerated daily) |
| `reports/integration-health.md` | Weekly integration health snapshot with week-over-week deltas |
| `reports/YYYY-MM-DD-*.md` | Dated point-in-time reports |

## How it works

A scheduled Claude Code routine sweeps the connected workspace (GitHub, Linear,
Notion, Gmail, Google Calendar, Google Drive, Slack, Atlassian, Zapier, Replit,
Figma, WorkOS, Superhuman Mail, Semrush, Spotify), regenerates the reports in
`reports/`, commits them here, and pushes a notification **only when something
needs a human decision** — at-risk deadlines, items awaiting approval, or a
previously healthy integration going dark. Quiet days produce commits, not pings.

## Notification policy

- **Notify**: at-risk deadline, approval/decision needed, integration regression, run failure.
- **Silent**: all clear, no change, empty workspace.
