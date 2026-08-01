# Integration Health Snapshot

**Baseline: 2026-07-03** · 15 systems probed read-only in parallel (workflow `wf_3c97ab93-1a1`, 15/15 returned, 0 errors).
Updated weekly by the Monday 08:11 Integration Health Audit; regressions trigger a notification.

## Scoreboard

| # | System | Status | Auth | Key facts |
| --- | --- | --- | --- | --- |
| 1 | Gmail | 🟢 Functioning | ✅ | ~201 threads last 7d, ~all unread; traffic is SaaS notifications; Superhuman AI labels actively triaging |
| 2 | Superhuman Mail | 🟢 Functioning | ✅ | 190 inbox threads (143 unread); Important split: 13 threads / **4 unread**; 11 labels incl. AI triage |
| 3 | Atlassian (Jira/Confluence) | 🟢 Functioning | ✅ | Site dgcrex.atlassian.net; 2 Jira projects: **KAN "My Operations Team"**, TC (template); full read/write scopes |
| 4 | Replit | 🟢 Functioning | ✅ | 1 app: **Capital Flywheel Agent**, last updated 2026-07-02 — most active real project found |
| 5 | Zapier | 🟢 Functioning | ✅ | 1 app enabled (Google Calendar, 15 actions); no custom skills yet; 9,000+ apps available |
| 6 | Google Drive | 🟢 Functioning | ✅ | Works, near-empty: 1 file ("12.pdf", 2026-06-20) |
| 7 | Figma | 🟢 Functioning | ✅ | Authenticated ("Rex's team", Starter); **View-only seat** limits write automation |
| 8 | GitHub (dgcrex/o) | 🟡 Was empty → now bootstrapped | ✅ | Empty at probe time; this repo's first commits landed today on `claude/blissful-tesla-uf77wk` |
| 9 | Google Calendar | 🟡 Functioning, empty | ✅ | 1 calendar (UTC tz), **0 events next 14 days** |
| 10 | Slack | 🟡 Functioning, empty | ✅ | Brand-new workspace: 3 channels, all created 2026-07-03; no #general |
| 11 | Linear | 🟡 Functioning, empty | ✅ | Workspace created today; 1 team, 0 projects, 4 stock onboarding issues (MUH-1…4) |
| 12 | Notion | 🟡 Functioning, empty | ✅ | 0 teamspaces, 0 content matching "project"; single user + bot |
| 13 | WorkOS | 🟠 Degraded | ✅ | Auth OK, but **MCP server disabled by an administrator** — query/mutate blocked |
| 14 | Semrush | 🔴 Unavailable | ✅ | Current plan **does not include MCP access** (semrush.com/mcp-access) |
| 15 | Spotify | 🔴 Unavailable | ❌ | **OAuth token expired** — needs re-authorization |

**Totals**: 7 functioning · 5 functioning-but-empty · 1 degraded · 2 unavailable.

## Action needed (connector fixes)

1. **Spotify** — reconnect in the connectors UI (token expired). ~1 minute.
2. **WorkOS** — an admin must re-enable the team's MCP server in the WorkOS dashboard.
3. **Semrush** — plan upgrade required for MCP access; decide whether SEO automation is worth it.
4. **Figma** (optional) — upgrade View seat to Edit if design-write automation is wanted.

## Delta log

- **2026-07-03**: baseline established. No prior snapshot to diff.
- **2026-07-29**: no full re-sweep performed (26 days stale, overdue for the weekly cadence this report claims). Partial spot-check this run surfaced a **regression**: Linear, Replit, and Superhuman Mail — all 🟢/🟡 functioning at baseline, and Linear specifically used successfully as recently as 2026-07-28 (PR #13) — now require re-authentication before any of their MCP tools can be used. Replit's loss is significant: it was the connector for Capital Flywheel Agent, "the most active real project in the workspace." A full 15-system probe is recommended to confirm scope and rule out further regressions.
- **2026-08-01**: still no full re-sweep (29 days stale). Partial spot-check: Linear, Replit, and Superhuman Mail **remain down for a 3rd consecutive run** — this is not a transient blip, it has now persisted since 2026-07-29. Notion and Jira/Confluence confirmed still reachable and functioning. WorkOS confirmed still has no dashboard account set up. Also new since 07-29: the daily dashboard-regeneration trigger itself skipped 2026-07-30 and 2026-07-31 before this run — first gap of its kind.
