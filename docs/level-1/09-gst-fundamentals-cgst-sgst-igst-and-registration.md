---
description: "GST Fundamentals: CGST, SGST, IGST & Registration — Goods and Services Tax (GST) is India's indirect tax on the supply of goods and services, levied at…"
---

# 09 · GST Fundamentals: CGST, SGST, IGST & Registration

**Goods and Services Tax (GST)** is India's indirect tax on the supply of goods and services, levied at each stage with credit for tax already paid. Before configuring it in TallyPrime (Level 2), you need the concepts. Rates and thresholds below are as of 2026 — always confirm the latest notifications on **gst.gov.in** and **cbic-gst.gov.in**.

## 1. How GST works

1. GST is a **value-added** tax: each business collects tax on its sales (**output tax**) and deducts tax paid on its purchases (**input tax credit, ITC**), paying the government the difference.
2. Example: Sri Sai Traders buys notebooks for ₹10,000 + 5% GST = ₹500 tax. It sells them for ₹14,000 + 5% = ₹700 tax. It pays ₹700 − ₹500 = **₹200** to the government — tax on the ₹4,000 value it added.
3. The final consumer bears the full tax; businesses act as collectors.

## 2. CGST, SGST/UTGST and IGST

1. **Intra-state supply** (seller and place of supply in the same state): tax split equally into **CGST** (Central) + **SGST** (State) — or UTGST in Union Territories. 18% = 9% CGST + 9% SGST.
2. **Inter-state supply** (different states) and imports: **IGST** at the full rate (18% IGST).
3. **Place of supply** rules decide which applies — for goods, generally where delivery ends; for many services, the recipient's location.
4. Sri Sai Traders (Telangana) selling to Hyderabad → CGST + SGST; selling to Bengaluru, Karnataka → IGST.

## 3. Rates and codes

1. Following the September 2025 rate rationalisation, most goods and services fall into **5%** (merit/essential items) or **18%** (standard), with **40%** for specified luxury and sin goods, plus **nil/exempt** items and special rates (e.g. 3% on gold). Check each item's current rate.
2. Goods are classified by **HSN** codes; services by **SAC** codes. Invoices must show HSN/SAC (4 digits for turnover up to ₹5 crore, 6 digits above, as currently required).
3. Using the wrong HSN or rate leads to short payment, interest and penalties.

## 4. Registration

1. Registration is mandatory when aggregate turnover exceeds **₹40 lakh** for goods suppliers (₹20 lakh in special category states) and **₹20 lakh** for service providers (₹10 lakh in special category states).
2. Some must register regardless of turnover: inter-state suppliers of goods, e-commerce sellers (with limited exceptions), casual taxable persons, those liable under reverse charge, and others.
3. Register on **gst.gov.in** with PAN, Aadhaar authentication, business proof and bank details; you receive a 15-character **GSTIN** (state code + PAN + entity number + check digit), e.g. `36ABCDE1234F1Z5` (36 = Telangana).
4. Small businesses may opt for the **Composition Scheme** (Level 2, Module 7).

## 5. Key returns (overview)

1. **GSTR-1** — details of outward supplies (sales), monthly by the 11th (or quarterly under QRMP).
2. **GSTR-2B** — auto-generated statement of ITC available from suppliers' filings.
3. **GSTR-3B** — summary return with tax payment, monthly by the 20th (staggered dates for quarterly filers).
4. **GSTR-9** — annual return.
5. Interest applies on late payment and late fees on late filing.

## Cheat sheet

| Term | Meaning |
|---|---|
| Output tax | GST on sales |
| ITC | Credit for GST paid on purchases |
| CGST + SGST | Intra-state supply |
| IGST | Inter-state supply, imports |
| HSN / SAC | Codes for goods / services |
| GSTIN | 15-character registration number |
| GSTR-1 / 3B | Sales details / summary + payment |

## How It Actually Works

GST taxes consumption at each stage but only on the value added, because every registered buyer offsets tax paid upstream through input tax credit. The split between CGST/SGST and IGST routes revenue to the right governments: IGST collected on inter-state sales is settled to the consuming state, preserving GST's destination-based design. The credit chain depends on matching — your ITC is backed by your supplier's reported sales (visible in GSTR-2B) — which is why accurate invoicing and timely supplier filing affect your own tax liability.

## Exercise

For Sri Sai Traders (Telangana), calculate GST and the tax split for: (1) sale of notebooks ₹20,000 at 5% to a Hyderabad shop; (2) sale of printer paper ₹50,000 at 18% to a Chennai buyer; (3) purchase of office chairs ₹30,000 at 18% from a Hyderabad supplier. Compute net GST payable for the month assuming full ITC eligibility. Decode GSTIN `36ABCDE1234F1Z5`.
