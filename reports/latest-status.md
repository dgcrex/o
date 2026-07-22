# Project Status Dashboard

**As of: 2026-07-22** · Regenerated from a live sweep of GitHub `dgcrex/o`, Linear, Notion, and Gmail.
**CronList**: 0 session-scoped jobs (all four in `automations/registry.md` expired ~2026-07-10, as every sweep since has confirmed). A separate, durable **"Daily 9am Briefing (Rex)"** automation is now sending email digests (seen 2026-07-20, 2026-07-21) — this is not in `automations/registry.md` and its schedule/owner session are unknown to this run.

## Active projects

| Project | Where | Deadline | Status | Progress | Notes |
| --- | --- | --- | --- | --- | --- |
| NO GAMES / VERANO 01 (NMG brand, clothing + music video launch) | Linear (`NMG`, `NO GAMES — Operational Integration` projects) + Notion ("Master Premiere Operating Bible") | none formally tracked | 🟢 Very active | early build-out | **Brand new since last sweep (7/20):** a full operating bible (Shopify/Neon/Klaviyo/webhooks/social engine) was built in Notion on 2026-07-21. MUH-30 ("CLOTHES NEED OT BE PRINTED...") sits under this project with an SLA that **breached 2026-07-20** — unactioned. |
| Personal-ops backlog (Obsidian import) | Linear, team MUH | none tracked | 🔴 Stalled | 0/30 done in 17 days | Backlog grew 26→30 issues since last sweep. 8 P0/Urgent issues remain, all blocked purely on facts/decisions only the account owner can supply. |
| GMP / IOPC Complaint | Notion + Linear MUH-21 | SAR "~mid-Jul" (unconfirmed) | 🔴 Blocked | 1 of 5 questions answered | Notion page still says SAR deadline was "verified from source letter and met," while Notion's own Notes field and MUH-21 both call the same date **unconfirmed/unverified**. Never reconciled since 2026-07-12. |
| DWP Universal Credit appeal (ref …744338) | Untracked (no Linear/Notion/Jira record) | reported 2026-07-18, now 4 days overdue | ⚠️ Unverified | — | **New finding this sweep:** searched Gmail directly for `744338` and for any `hmcts`/`dwp` sender — the only matches are this automation's own past summary emails. No original DWP/HMCTS correspondence is visible in this account. Before treating this as the top fire, confirm the source letter actually exists and is in this mailbox (or another one). |
| Ops Automation Hub (this repo) | GitHub `dgcrex/o` | rolling | 🟡 At risk | — | **10 open PRs** (#1–#9 plus this one) now propose the same dashboard-regeneration content, all unmerged since 2026-07-05. Every sweep for 17 days has flagged this and recommended a single triage pass; none has happened. |
| Held Gmail drafts | Gmail | — | 🔴 Stalled | — | 50+ unsent drafts date back to 2026-07-03, including drafted letters to external recipients (`justice.gov.uk`, `greatermanchester-ca.gov.uk`, `trafford.gov.uk`, `mitie.com`) that have never been sent. Materially larger than the "12 held drafts" figure cited in PRs #7–#9. |
| Capital Flywheel Agent | Replit | none set | ⚪ Unknown | unknown | Replit connector requires reauth; could not be checked this sweep (also reported "suspended" in the 2026-07-20 briefing email — unconfirmed independently). |
| My Operations Team (KAN) | Jira | none set | ⚪ Dormant | 0% | No real issues filed; unchanged since baseline. |

## Awaiting your decision

1. **PR triage** — 10 open duplicate PRs (#1–#9 + this one) on `dgcrex/o`. Recommend merging whichever has the freshest data and closing the rest; no automation should do this unattended.
2. **Verify the DWP appeal deadline is real** — no source email found in this mailbox despite 12+ days of escalating alerts about it (ref …744338).
3. **MUH-21** — 4 of 5 GMP escalation questions still need answers only you can supply.
4. **MUH-30 / NMG clothing** — SLA breached 2026-07-20; confirm priority/legitimacy of the wider "NO GAMES" build-out that appeared 2026-07-21.
5. **Reconcile the GMP/IOPC SAR-deadline contradiction** between Notion and Linear (unresolved since 2026-07-12).
6. **Clear the Gmail draft backlog** — several are addressed to external government/legal recipients and have sat unsent for 2–3 weeks.
7. **Carried forward, unresolved since baseline**: WorkOS re-enable, Semrush MCP plan, durable-scheduling decision for the four expired automations, and independent verification of the two previously-flagged social-engineering emails.

## Automation runs

| Automation | Last run | Next scheduled | Recent findings |
| --- | --- | --- | --- |
| Project status dashboard (this task) | 2026-07-22 (this run) | on next trigger (session-scoped; not durable) | See above. |
| "Daily 9am Briefing (Rex)" | 2026-07-21 08:11 (also seen 2026-07-20) | unknown — not registered in `automations/registry.md` | Reported DWP overdue, Replit suspended, Adobe payment failed. |
| 15-system integration health sweep | 2026-07-03 (baseline) | none — job expired | Not re-run this session; WorkOS/Semrush/Spotify still unresolved. |
| Morning Ops Brief / Midday Pulse / EOD Status Dashboard (registry jobs) | none since baseline | none — all 4 session-scoped jobs expired ~2026-07-10 | Superseded in practice by manual dashboard-regeneration PRs and the external 9am briefing email. |
