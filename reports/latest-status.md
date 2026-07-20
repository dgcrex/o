# Project Status Dashboard

**As of: 2026-07-20** · Regenerated from a live sweep of GitHub `dgcrex/o`, Linear, Notion, and Gmail.
(`CronList` confirms 0 scheduled jobs — unchanged since ~2026-07-10; this remains a manual/on-demand run, not the automated EOD job.)

## Active projects

| Project | Where | Deadline | Status | Progress | Notes |
| --- | --- | --- | --- | --- | --- |
| DWP UC appeal response (ref …744338) | Gmail/HMCTS | **was due 2026-07-18 — now 2 days overdue** | 🔴 Blown, unactioned | — | No HMCTS/DWP correspondence found since the 07-18 deadline email. No reply, extension, or tribunal update on record. |
| Linear personal-ops backlog ("Muhammad Ikram" / Rex) | Linear | mixed, several P0 | 🔴 Stalled | 0/30 done | Grew from 26→30 issues; still zero completions in 15 days. See MUH-21 and MUH-30 below. |
| ├─ MUH-21: Answer 5 GMP escalation questions | Linear | referenced SAR ~13 Jul (unverified) | 🟡 Partially answered | 1/5 | New comment 2026-07-19 17:19 from "Rex": solicitor responded but can't help, no referral known. 4 of 5 questions (recording ref, outcome letter, solicitor detail, SAR received) still unanswered; issue still in Todo. |
| ├─ MUH-30: "NMG clothing/logos" (new, 2026-07-19) | Linear + new repo `dgcrex/MINEDOBNS` | none | ⚠️ Anomalous | — | Created same 17:1x window as a bulk timestamp touch across the whole backlog. Off-topic vs. the personal-ops set, aggressive all-caps tone. Flagged as possible noise/scope creep — recommend the account owner confirm this is legitimate before anyone builds on it. |
| Notion "GMP / IOPC Complaint" page | Notion | — | 🟡 Unreconciled | — | Unchanged since 07-12. "Definition of Done" says SAR deadline "verified and met"; its own Notes field says the same deadline is "UNCONFIRMED... verify before any action." Contradicts MUH-21's still-open unverified date. |
| 12 held Gmail drafts ("Obsidian Command/HELD — Awaiting YES-NO") | Gmail | review was due 2026-07-08 | 🔴 12 days overdue | untouched | 15+ drafts dated 07-05–07-08, none sent or deleted, no newer activity. |
| Ops Automation Hub (this repo) | GitHub `dgcrex/o` | rolling | 🟡 At risk | scaffolded | Repo itself fine; the 4 documented automations have been fully lapsed since ~07-10 (session-scoped cron expired, never made durable). |
| Capital Flywheel Agent | Replit | none set | ⚪ Unknown | unknown | Not re-probed this run (Replit needs re-auth); last known update 2026-07-02. |
| My Operations Team (KAN) | Jira | none set | ⚪ Unchanged | 0% | No real issues filed as of last probe. |

## Awaiting your approval / decision

1. **DWP UC appeal (ref …744338) — now overdue.** Highest-priority item in the workspace. Needs to be confirmed handled (or escalated) outside this workspace; no automation can act on this for you.
2. **MUH-21 — 4 of 5 GMP escalation questions still unanswered.** Only you hold: the recording reference, outcome letter, solicitor engagement detail, and SAR-received confirmation.
3. **Reconcile the SAR-deadline conflict** between Notion (says "met") and Linear MUH-21 (still open, unverified date) — one of the two is wrong.
4. **MUH-30 anomaly** — confirm whether this new issue + repo (`dgcrex/MINEDOBNS`) is something you actually created/intended, given its off-topic content and the bulk-timestamp pattern it appeared alongside.
5. **12 held Gmail drafts**, 12 days overdue for review — approve/reject or archive.
6. **PR backlog: 8 open, unmerged, draft PRs (#1–#8)**, all proposing the same dashboard-regeneration content since 2026-07-05, none merged or closed. This PR (likely #9) continues the pattern. Recommend a single triage pass: merge the freshest (or this one) and close the rest, or explicitly tell the automation to stop opening new PRs until one is merged.
7. **Durable scheduling / connector decisions** (WorkOS, Semrush, Spotify re-auth, choice of deadline source-of-truth) — all carried forward unresolved since baseline, no automation currently running to re-flag them (all 4 session cron jobs lapsed ~07-10).

## Tasks/automations set to auto-iterate

| Automation | Registered schedule | Last actual run | Next scheduled | Recent findings/errors |
| --- | --- | --- | --- | --- |
| Morning Ops Brief | daily 06:57 | never confirmed run | — (cron lapsed) | Session-scoped cron expired ~07-10; not recreated as a durable routine. |
| Midday Pulse | weekdays 12:21 | never confirmed run | — (cron lapsed) | Same as above. |
| EOD Status Dashboard | daily 17:34 | none since baseline; all updates since have been manual/on-demand runs (this one included) | — (cron lapsed) | `CronList` returns 0 scheduled jobs. |
| Weekly Integration Health Audit | Mondays 08:11 | 2026-07-03 (baseline only) | — (cron lapsed) | `reports/integration-health.md` is 17 days stale; last known state: WorkOS degraded (admin must re-enable), Semrush unavailable (plan upgrade needed), Spotify unavailable (token expired). |

**No automation in this workspace is currently live.** Every dashboard update since 2026-07-05 (10 in a row, including this one) has been a manual/on-demand regeneration, not the scheduled job described in `automations/registry.md`.

## Summary

- **On track:** Nothing new — this workspace has had no completed work in 15 days.
- **At risk:** MUH-21 GMP questions (partially moving, still 80% unanswered), Notion/Linear SAR-deadline contradiction, connector decisions (WorkOS/Semrush/Spotify), automation durability.
- **Needs immediate attention:** the DWP UC appeal deadline (blown 2 days ago, no evidence of action), the 8-PR backlog with zero merges, and the MUH-30 anomaly, which should be verified as legitimate before it's built on.
