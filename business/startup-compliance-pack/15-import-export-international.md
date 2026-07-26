# 15 — INTERNATIONAL IMPORT / EXPORT

**Status:** DRAFT · **Risk:** HIGH (customs/duty liability) · **Approval:** L4 · **Timing:** "Later — before first shipment" per matrix

## 1. Registrations — before first shipment `ACTION REQUIRED`
- [ ] **EORI number** (GB prefix) — free from HMRC, needed to import/export; confirmation to folder 10.
- [ ] If selling into the EU later: EU EORI/IOSS decision — **L5** when it arises.
- [ ] Duty-deferment or postponed VAT accounting election (import VAT on the VAT return instead of at the border — needs VAT registration, doc 06).

## 2. Per-product customs schedule (build once, reuse)
| Field | Notes |
|---|---|
| Commodity/HS code | Classify honestly via UK Trade Tariff — garments typically ch. 61/62; hardware/trims may differ. Misclassification = back-duty + penalties |
| Duty rate + origin | Country of origin drives rate; check UK trade agreements |
| VAT at import | 20% standard on garments |
| Restrictions | Fur/leather/species (CITES), chemical limits (see REACH note) |

## 3. Shipment file (one per shipment — folder 10)
Commercial invoice (true value — **never under-declare**, even if supplier offers) · packing list · transport doc/AWB · customs entry (C88/CDS) · duty/VAT payment or PVA statement · origin records. Retention: keep 6 years.

## 4. Incoterms + who pays what
Supplier quotes: prefer **FOB** (you control freight/agent) over EXW (all risk yours from factory floor). Customer sales international: **DDP** (you pay duties — clean customer experience, price it in) vs **DAP** (customer pays at door — state it loudly in checkout, doc 05). Decision: `PLACEHOLDER`.

## 5. JD/Footasylum route interaction (route-mandatory layer)
Import documentation feeds the wholesale pack: REACH declarations for inks/dyes/finishes travel with supplier shipping docs (folder 04); SMETA/SEDEX factory audit reports collected at supplier onboarding (doc 07); GS1 company prefix licensed → EAN-13/GTIN assigned per SKU before intake (folder 05). **Retailer-entry requirements, not universal law — mandatory for this project.**

## 6. Customs agent
First shipments: use a freight forwarder/customs broker as **direct representative** (you remain liable — accuracy still yours). Representation letter to folder 10.

## Approval route — schedules/files L1 → EORI + registrations **L4 HOLD** → first international PO/shipment booking **L4** → EU structures/IOSS **L5**.
