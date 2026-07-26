# [NOG][AI] MASTER STATE SUMMARY — BASELINE (WEEK 0, w/c 27 Jul 2026)

> Paste this block into the Friday `[NOG][AI][ACTIVE] Weekly State Summary` event description,
> update it every Friday, and paste the updated block into any AI session as the single source of truth.

```
[NOG][AI] STATE SUMMARY — 2026-07-31 (Week 0)

1. ACTIVE OUTPUTS:
   - 1920x2400 px 20-mark master logo sheet — status: NOT STARTED
   - 1920x2400 px August garment placement/trim/colour/technical spec sheet — status: NOT STARTED
   - Everything else: HOLD

2. GATE STATUS (G1-G5):
   - G1 Welfare/benefits written advice + DWP disclosure: OPEN (not DONE)
   - G2 Commercial registered office live: OPEN
   - G3 Business structure decision: BLOCKED (needs G1)
   - G4 Incorporation filing: BLOCKED (needs G1-G3 + APPROVE)
   - G5 Business banking: BLOCKED (needs G4 + APPROVE)

3. BLOCKERS:
   - No written LCWRA/UC advice yet (blocks G3-G5, trademark, all filings)
   - No registered-office contract yet (blocks incorporation address)

4. EVIDENCE IDs (NoG-###):
   - None issued yet. First expected: NoG-001 = welfare advice note,
     NoG-002 = DWP disclosure record, NoG-003 = registered-office contract.

5. DECISIONS REQUIRED:
   - Approve registered-office provider purchase (L3)
   - Ltd vs sole trader (after G1 advice, L5 input)
   - Confirm SIC set + trademark classes

6. REVERSIBLE AI TASKS (safe to run any time):
   - Draft welfare-advice request text (held draft)
   - Provider shortlists (registered office, bank, store platform, PSP)
   - Bootstrap financial model skeleton; policy drafts; supplier
     due-diligence templates

7. NEXT ACTION (single, fastest):
   - Book Citizens Advice / welfare-rights appointment for written
     LCWRA/directorship advice (Gate 1)

8. DEADLINES (14-day view):
   - No external deadlines owed by NOG in this window.
   - Fixed anchors ahead: bail return 27 Aug · tenancy end 4 Sep ·
     protected period to 15 Sep (ops resume 16 Sep)

9. OWNER: Rex (all gates; no delegates registered)

10. ACCEPTANCE TEST (this week): G1 appointment booked AND calendar
    imported with statuses intact = week PASSES.

11. STATUS VERDICT: PASS-WITH-GAPS — system deployed, all gates open,
    nothing external committed.
```

## Update rules
- Only the Monday command review (or an explicit user decision) flips a gate tag `[BLOCKED]` → `[ACTIVE]` → `DONE` — edit the event title so the calendar always shows status truth.
- New evidence gets the next NoG-### number and is logged in field 4 AND in pack doc 17.
- If a week ends with no update, the last pasted block remains authoritative — never reconstruct state from memory.
