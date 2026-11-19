---
description: "GSTR-1 and GSTR-3B Returns — Every regular GST taxpayer files two core returns: GSTR-1 (details of sales) and GSTR-3B (summary and payment). This module…"
---

# 04 · GSTR-1 and GSTR-3B Returns

Every regular GST taxpayer files two core returns: **GSTR-1** (details of sales) and **GSTR-3B** (summary and payment). This module prepares both from TallyPrime and walks through filing on the portal. Confirm current due dates and forms on gst.gov.in.

## 1. Due dates and periodicity

1. **GSTR-1**: monthly by the **11th** of the next month; or quarterly under **QRMP** (turnover up to ₹5 crore) by the 13th after the quarter, with optional **IFF** for B2B invoices in the first two months so buyers get credit sooner.
2. **GSTR-3B**: monthly by the **20th**; QRMP taxpayers file quarterly (22nd or 24th depending on state) and pay monthly via **PMT-06**.
3. Late fees and 18% interest on late tax apply — file on time even with nil activity (nil returns can be filed by SMS).

## 2. Prepare GSTR-1 in TallyPrime

1. **Alt+G → GSTR-1** for the month.
2. Review **Return View**: B2B invoices, B2CL, B2CS, exports, credit/debit notes (registered and unregistered), nil/exempt supplies, advances, **HSN summary** and **documents issued**.
3. Resolve **uncertain transactions** (missing GSTIN, HSN, place of supply, rate) before export.
4. Export the return as JSON (**Alt+E**) and upload to the portal's offline tool, or upload directly with TallyPrime's connected GST features.
5. On the portal: **Returns → GSTR-1 → Prepare online/upload**, check summary, **file with DSC or EVC (OTP)**.

## 3. Prepare GSTR-3B

1. **Alt+G → GSTR-3B** for the same month.
2. Key tables:
   - **3.1** Outward taxable supplies (taxable value and tax), zero-rated, nil/exempt, inward supplies under reverse charge.
   - **3.2** Inter-state supplies to unregistered persons, composition dealers (by state).
   - **4** Eligible ITC — from imports, RCM, and all other ITC — minus reversals; matched to GSTR-2B.
   - **5** Exempt/nil/non-GST inward supplies.
   - **6** Payment of tax.
3. On the portal, values are **auto-populated** from your GSTR-1 and GSTR-2B; compare them with TallyPrime's computation and resolve differences. Recent portal changes restrict editing auto-populated liability — correct errors through GSTR-1A/next GSTR-1 amendments as the portal guides.

## 4. Pay the tax

1. Worked example for the month: Output CGST ₹48,000, SGST ₹48,000, IGST ₹62,000. Eligible ITC: CGST ₹31,000, SGST ₹31,000, IGST ₹70,000.
2. Set-off order: **IGST credit** first against IGST liability, then CGST and SGST (in any order or proportion); **CGST credit** against CGST then IGST; **SGST credit** against SGST then IGST. CGST and SGST credits can't be used against each other.
3. IGST credit ₹70,000: ₹62,000 against IGST, remaining ₹8,000 against CGST → CGST liability left ₹40,000 − ₹31,000 CGST credit = ₹9,000 cash; SGST ₹48,000 − ₹31,000 = ₹17,000 cash.
4. Deposit cash via **PMT-06** challan (UPI, net banking, NEFT/RTGS) into the electronic cash ledger, then offset in GSTR-3B and file.
5. In TallyPrime, record the set-off with a **Journal** (output vs input tax ledgers) and the payment with a **Payment** voucher (Stat Payment details: GST, period).

## Cheat sheet

| Return | Content | Due (monthly) |
|---|---|---|
| GSTR-1 | Invoice-level sales | 11th |
| GSTR-3B | Summary + tax payment | 20th |
| IFF | B2B invoices (QRMP months 1–2) | 13th |
| PMT-06 | Monthly payment (QRMP) | 25th |
| Set-off | IGST → CGST/SGST; CGST ↛ SGST | |

## How It Actually Works

GSTR-1 is the source data the system uses to build every buyer's GSTR-2B and to auto-populate your own GSTR-3B liability, so accuracy in GSTR-1 drives everything else. GSTR-3B is where tax is actually paid: liabilities are offset first using credits in a legally prescribed order (IGST credit is used first because it's shared between the Centre and states), with the balance paid in cash. TallyPrime's role is to make the books, the returns and the payment entries agree.

## Exercise

For Godavari Wholesale Mart, generate GSTR-1 for your Level 2 transactions, fix any uncertain items and export JSON. Prepare GSTR-3B, compute the set-off for the month using your figures, and record the set-off journal and the cash payment voucher.
