---
description: "Reverse Charge & the Composition Scheme — Normally the supplier charges and pays GST. Under the reverse charge mechanism (RCM), the recipient pays…"
---

# 07 · Reverse Charge & the Composition Scheme

Normally the supplier charges and pays GST. Under the **reverse charge mechanism (RCM)**, the recipient pays instead. Small businesses may also choose the simplified **Composition Scheme**. This module handles both in TallyPrime. Rules and lists are as of 2026 — verify current notifications.

## 1. Reverse charge — when it applies

1. **Notified services** (examples): goods transport agency (GTA) services to specified recipients (when GTA hasn't opted to pay tax itself), legal services by advocates to businesses, services by directors to the company, sponsorship services to body corporates, security services by non-corporate suppliers to registered persons, and renting of commercial property by an unregistered person to a registered person.
2. **Notified goods** (examples): cashew nuts (not shelled), tendu leaves, certain tobacco leaves, silk yarn, raw cotton, when supplied by specified suppliers.
3. **Imports of services** are generally under RCM (IGST paid by the importer).
4. Specified procurements from unregistered suppliers by certain sectors (e.g. real estate promoters) also attract RCM.

## 2. Accounting for RCM

1. The recipient issues a **self-invoice** (for supplies from unregistered persons) and a **payment voucher** to the supplier.
2. Tax under RCM must be paid in **cash** (electronic cash ledger) — ITC can't be used to pay it.
3. The recipient can then claim the same amount as **ITC** if eligible, so the net cost is usually cash flow timing.
4. Report in GSTR-3B **Table 3.1(d)** (liability) and **Table 4** (ITC).

## 3. RCM in TallyPrime

1. Create the expense/service ledger (e.g. "Legal Fees") with GST details: SAC, rate and **Applicable for reverse charge: Yes**.
2. Record the purchase voucher from the supplier; TallyPrime calculates the RCM tax and marks the liability.
3. Use TallyPrime's **Stat Adjustment** journal ("Increase of Tax Liability & Input Tax Credit" for reverse charge) — or the automated RCM handling in recent releases — to book tax liability and ITC.
4. Example: advocate fees ₹50,000 (intra-state, 18%) → RCM liability CGST ₹4,500 + SGST ₹4,500; pay ₹9,000 in cash with GSTR-3B; claim ₹9,000 ITC.

## 4. Composition Scheme

1. Eligibility: aggregate turnover up to **₹1.5 crore** (₹75 lakh in special category states) for goods suppliers and restaurants; up to **₹50 lakh** for eligible service providers.
2. Tax rates on turnover: **1%** for manufacturers and traders (0.5% CGST + 0.5% SGST), **5%** for restaurants not serving alcohol, **6%** for service providers.
3. Restrictions: can't collect tax from customers (issue a **Bill of Supply**), can't claim ITC, can't make inter-state outward supplies of goods or sell through most e-commerce operators, and must display "composition taxable person" on signboards and bills.
4. Returns: **CMP-08** quarterly statement-cum-challan and **GSTR-4** annual return.
5. In TallyPrime, set registration type **Composition** in GST details; sales print as Bills of Supply and the composition tax is computed on turnover.

## Cheat sheet

| Topic | Key rule |
|---|---|
| RCM payer | Recipient |
| RCM payment | Cash only; ITC claimable if eligible |
| Self-invoice | For purchases from unregistered under RCM |
| GSTR-3B | 3.1(d) liability, 4 ITC |
| Composition limit | ₹1.5 crore (goods), ₹50 lakh (services) |
| Composition rates | 1% / 5% / 6% |
| Composition returns | CMP-08 quarterly, GSTR-4 annual |

## How It Actually Works

RCM shifts the tax obligation to the recipient where collecting from many small or unregistered suppliers would be impractical; requiring cash payment ensures real revenue enters the system before the recipient claims credit. The Composition Scheme trades simplicity for limits: low tax on turnover with minimal compliance, but no credit chain — which makes composition dealers less attractive suppliers for businesses that want ITC, a real commercial consideration when choosing the scheme.

## Exercise

Record for Godavari Wholesale Mart: advocate fees ₹50,000 under RCM, GTA freight ₹12,000 under RCM at 5%, and rent ₹40,000 for a godown from an unregistered owner. Compute the RCM liability, the cash payable and the ITC claimable. Then calculate quarterly composition tax for a small trader with ₹28 lakh turnover in the quarter.
