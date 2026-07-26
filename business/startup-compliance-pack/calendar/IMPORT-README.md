# NO GAMES — OPERATIONS calendar: import instructions

**File:** `NoGames_OS.ics` · one import, whole system lands intact (RRULEs + EXDATEs included).
Format is ICS, not CSV — Google's CSV import drops recurrence and notification behaviour.

## Exact sequence (10 minutes, do in this order)

1. **Create the calendar** — Google Calendar → Settings → Add calendar → Create new calendar:
   Name `NO GAMES — OPERATIONS` · time zone Europe/London → Create. Then set its colour to
   dark/black in the sidebar and leave it private (default).
2. **Set default notifications BEFORE importing** — Settings → NO GAMES — OPERATIONS →
   Event notifications: add three: **7 days · 48 hours · 2 hours**. Imported events inherit
   calendar defaults, which is why this comes before step 3.
3. **Import** — Settings → Import & export → select `NoGames_OS.ics` →
   **destination calendar: NO GAMES — OPERATIONS** → Import. Expect ~18 events created.
4. **Verify status truth** — check that: the only `[ACTIVE]` work items are the two design
   sheets (Tuesday block); Gates 3–5, both filings, and all APPROVE events show `[BLOCKED]`;
   no NOG blocks appear on 27 Aug (Thu) or between 4–15 Sep.
5. **Paste the AI State Summary** — open Friday 31 Jul `[NOG][AI][ACTIVE] Weekly State Summary`
   and paste the baseline block from `AI-STATE-SUMMARY.md` into the description.

## What's encoded

- **Weekly rhythm from Mon 27 Jul 2026** (Europe/London, DST-safe): Mon 10:00–11:30 command
  review · Tue design (two active deliverables only) · Wed compliance/evidence · Thu website ·
  Fri finance + 14:00 AI State Summary · Sun 18:00 fourteen-day conflict check. Max two priority
  blocks daily; 30-min buffers noted in each event.
- **Five gates** as all-day banners: G1 welfare/benefits advice (27–28 Jul, ACTIVE) ·
  G2 registered office (28–29 Jul, ACTIVE) · G3 structure decision (31 Jul, BLOCKED) ·
  G4 incorporation (target 10 Aug, BLOCKED) · G5 banking (target 17 Aug, BLOCKED) ·
  plus trademark filing (target 18 Aug, BLOCKED). Target dates are provisional and move only
  by explicit Monday-review decision — never silently compressed.
- **48-hour APPROVE events** before each irreversible step (incorporation 8 Aug, banking 15 Aug,
  trademark 16 Aug) — no same-day decide-and-act.
- **Constraint banners:** bail return 27 Aug · tenancy end 4 Sep · protected legal/tribunal
  period 4–15 Sep with all NOG blocks pre-excluded (EXDATEs); ops resume Wed 16 Sep.

## Status ladder on event titles
`[BLOCKED]` → `[ACTIVE]` → `DONE` (edit the title when a gate flips — the calendar must always
show current truth). Gates flip only at the Monday command review or by explicit decision.
