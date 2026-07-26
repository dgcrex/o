# 14 — PAYMENTS COMPLIANCE

**Status:** DRAFT · **Risk:** MEDIUM · **Approval:** L4 (PSP agreements)

## 1. Payment stack (decision — `PLACEHOLDER`)
Score: Shopify Payments/Stripe (cards, wallets) + PayPal (buyer trust) + Klarna/BNPL (streetwear conversion — note FCA-regulated messaging rules). Criteria: fees ~1.5–3% + fixed, payout timing to doc 03 account, chargeback tooling, multi-currency support for international orders.

## 2. Compliance duties

- [ ] **PCI-DSS**: use hosted checkout/PSP fields only — **never store card numbers**; complete the PSP's SAQ-A attestation; file in folder 06.
- [ ] **Strong Customer Authentication (3DS2)** enabled — PSP default; do not disable.
- [ ] **PSP onboarding (KYB)**: they will verify company number, directors, website legal pages (doc 05) — pack docs 01–02 feed this; mismatched details = frozen payouts.
- [ ] **Refunds**: 14-day cancellation refunds within 14 days of return (doc 05); refunds always to the original payment method.
- [ ] **Chargebacks**: respond by deadline with evidence pack (order, T&Cs acceptance, tracking + signature); keep win/loss log (folder 08 of tree = Orders).
- [ ] **AML posture**: retail goods sales are not FCA-regulated activity, but watch red flags — large resale-pattern orders, mismatched cards/addresses, requests to refund to a different account (**never do this** — classic laundering pattern). Log and refuse.
- [ ] **Payouts to contributors** (models/artists — doc 12 §4): bank transfer against invoice only; international payments need withholding-tax check (**L5** first time per country).

## 3. Records
PSP agreements + fee schedules · monthly payout reconciliations to accounting (doc 06) · chargeback files · fraud-refusal log. Retention 6 years.

## Approval route — stack comparison L1 → PSP applications/agreements **L4 HOLD** → payout of funds always **L4**.
