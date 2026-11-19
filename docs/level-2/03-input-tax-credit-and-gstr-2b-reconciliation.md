---
description: "Input Tax Credit & GSTR-2B Reconciliation — Input tax credit (ITC) lets you reduce GST payable by the GST you paid on business purchases. It's valuable —…"
---

# 03 · Input Tax Credit & GSTR-2B Reconciliation

**Input tax credit (ITC)** lets you reduce GST payable by the GST you paid on business purchases. It's valuable — and closely policed. This module covers eligibility, blocked credits, and reconciling your books with **GSTR-2B** every month.

## 1. Conditions for claiming ITC

1. You hold a valid **tax invoice** or debit note.
2. You've **received** the goods or services.
3. The supplier has **reported the invoice in their GSTR-1** and it appears in your **GSTR-2B**.
4. The supplier has **paid the tax** to the government.
5. You've **filed your GSTR-3B**.
6. Claim within the time limit: by **30 November** following the end of the financial year (or the annual return date, if earlier).
7. Pay the supplier within **180 days** of the invoice date; otherwise reverse the ITC (with interest) and re-claim when paid.

## 2. Blocked credits (Section 17(5) — examples)

1. Motor vehicles for personal transport (with exceptions such as dealers, driving schools, passenger transport businesses).
2. Food and beverages, outdoor catering, beauty treatment, health services, club memberships — unless used for making the same outward supply or provided under a legal obligation.
3. Works contracts and goods/services for constructing immovable property (other than plant and machinery) on your own account.
4. Goods lost, stolen, destroyed, written off or given as free samples or gifts.
5. Goods or services for personal consumption.
6. In TallyPrime, record ineligible ITC on purchase ledgers/items marked **Ineligible** so it isn't claimed.

## 3. Understanding GSTR-2B

1. **GSTR-2B** is a static monthly statement on the GST portal (generated around the 14th) showing ITC available from suppliers' GSTR-1/IFF filings, imports and more.
2. It shows ITC **available** and **not available** (e.g. late or ineligible) and supplier details.
3. The **Invoice Management System (IMS)** on the portal lets recipients **accept, reject or keep pending** inward invoices before GSTR-2B is finalised — review it monthly.

## 4. Reconcile in TallyPrime

1. Download GSTR-2B (JSON) from the portal, or use TallyPrime's **connected GST** features to fetch it directly.
2. In TallyPrime: **Alt+G → GSTR-2B Reconciliation** (or GSTR-2A/2B under the GST reports menu) → **Import** the file.
3. TallyPrime matches portal records with your purchase vouchers by GSTIN, invoice number, date and amounts, showing: **Matched**, **Partially matched** (e.g. amount or date differs), **Available only in books**, **Available only in portal**.
4. Investigate each mismatch:
   - Only in books → supplier hasn't filed; follow up before claiming.
   - Only in portal → you missed recording the purchase (or it's not yours — reject in IMS).
   - Partial → typo in invoice number/date or different amounts; correct your voucher or ask the supplier to amend.
5. Claim ITC in GSTR-3B only for eligible, matched invoices.

## Cheat sheet

| Check | Rule |
|---|---|
| Documents | Valid invoice, goods/services received |
| Supplier compliance | In GSTR-2B, tax paid |
| Time limit | 30 Nov of next FY (or annual return date) |
| Payment | Within 180 days or reverse |
| Blocked | Sec 17(5) items |
| Monthly | Review IMS, reconcile 2B with books |

## How It Actually Works

The GST system links every buyer's credit to a seller's declared sale. GSTR-2B is the portal's authoritative view of what the government will accept as your ITC for the period, built from your suppliers' filings — and GSTR-3B's ITC claims are compared against it. Regular reconciliation turns that system into a control: it catches supplier non-compliance early (while you can still press them to file) and prevents excess claims that would attract interest and penalties.

## Exercise

Create a sample GSTR-2B reconciliation for Godavari Wholesale Mart with eight purchase invoices: five that match, one only in books, one only in the portal, and one with a different invoice number. Write the action for each, calculate eligible ITC for the month, and identify which of these purchases would be blocked: a staff lunch, a delivery van for goods transport, a laptop, and gifts to dealers.
