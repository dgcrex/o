# 11 — DATA PROTECTION (UK GDPR / DPA 2018 / PECR)

**Status:** DRAFT · **Risk:** HIGH (fines + reputational) · **Approval:** L4 (ICO registration, policy publication)

## 1. Registrations & roles

- [ ] **ICO registration (data protection fee)** — required for almost every trading company: Tier 1 £52/year for most small businesses (£40 by direct debit — verify current fee). `ACTION REQUIRED` after incorporation.
- [ ] Controller = the company. No DPO legally required at this scale, but name one accountable person: the director. `PLACEHOLDER` (name).

## 2. Data inventory (Record of Processing Activities — keep even though small)

| Data set | Source | Lawful basis | Retention |
|---|---|---|---|
| Customer orders (name, address, contact, order history) | Store checkout (05) | Contract | 6 years (tax evidence) |
| Payment data | PSP handles card data — never store card numbers (14) | Contract | PSP-side |
| Marketing list (email/SMS) | Opt-in at checkout/signup | Consent (PECR: soft opt-in only for own similar products, with opt-out every message) | Until unsubscribe + suppression record |
| Giveaway entrants | Entry form (13) | Consent/contract (promotion terms) | 6 months post-draw, winners 6 years (audit) |
| Models/artists (contracts, images, payment details) | Bookings (12) | Contract + legitimate interests | 6 years post-contract |
| Model images incl. identifiable people | Shoots | Contract + release (12); if any biometric/special category arises → explicit consent | Per release terms |
| Website analytics/cookies | Site (05) | Consent (PECR) for non-essential | Per tool, minimise |
| International transfers (suppliers/PSPs outside UK) | Docs 07/14/15 | Adequacy or IDTA/SCCs — list each processor | — |

## 3. Documents to publish/hold — `ACTION REQUIRED` (drafts on request, T2)

1. **Privacy policy** (public, on site): who you are, what you collect, why, lawful bases, sharing (PSP, courier, email platform), international transfers, retention, rights, complaint route to ICO.
2. **Cookie policy + banner** with real reject option.
3. **Internal data protection policy** (one page: minimisation, access, passwords/2FA, device encryption, staff rules).
4. **Retention schedule** (table above, adopted formally).
5. **Breach log + breach response plan**: contain → assess → if risk to individuals, report to ICO within **72 hours** → notify individuals if high risk → record everything even if not reportable.
6. **SAR procedure**: subject access requests answered within one month, free; identity check first; log kept.
7. **Processor list + agreements**: every tool touching personal data (store platform, email tool, PSP, courier, cloud drive) with a DPA in place — list is `PLACEHOLDER` until stack chosen.

## 4. Model/artist imagery — specific rules (cross-ref doc 12)

- Identifiable images of people = personal data; the release in doc 12 is the processing record.
- Right to withdraw: releases must say what happens to already-published material (contract survives for published works; future use stops).
- Never publish a model's personal details (real name if working under alias, contact info, location patterns) without written consent — safety issue, not just compliance.

## 5. Security baseline (do these this week)

Unique passwords + 2FA on store/bank/email/PSP · device encryption on · auto-updates on · least-access sharing on cloud folders · quarterly access review logged in audit loop (08).

## Approval route
- Drafting all policies: L1/T2.
- ICO registration + publishing policies: **L4 — HOLD.** Complex questions (special-category data, minors' data): **L5.**
