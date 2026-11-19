---
description: "Project — A GST-Compliant Month for a Wholesaler — Combine Level 2: run a full GST month for a wholesaler — setup, invoicing, notes, ITC reconciliation,…"
---

# 10 · Project — A GST-Compliant Month for a Wholesaler

Combine Level 2: run a full GST month for a wholesaler — setup, invoicing, notes, ITC reconciliation, RCM, e-documents, receivables and returns — in TallyPrime. Use a new company, *Krishna Electricals*, Pune (Maharashtra, GSTIN state code 27), regular taxpayer with monthly returns.

## 1. Setup

1. Create the company with GST, bill-wise details, cost centres (branches: Pune, Nashik) and inventory.
2. Tax ledgers (input/output CGST, SGST, IGST), GST-applicable sales/purchase ledgers, RCM-applicable Legal Fees and GTA Freight ledgers.
3. Parties: four customers (two Maharashtra registered, one Gujarat registered, one unregistered retail), three suppliers (one inter-state).
4. Items with HSN codes and current rates: LED panels, MCB switches, copper wire coils, ceiling fans, extension boards (look up actual rates on the CBIC rate finder).

## 2. Transactions

1. Five purchases (one inter-state), with supplier invoice numbers.
2. Eight sales: intra-state B2B, inter-state B2B, B2C retail, one inter-state B2C above ₹1 lakh; allocate to branches.
3. One sales return credit note and one pre-agreed discount credit note.
4. One purchase return.
5. RCM: advocate fees ₹30,000 and GTA freight ₹8,000.
6. Receipts: two full, one partial (Agst Ref), one advance; supplier payments within terms.
7. Assume turnover above ₹5 crore: prepare e-invoice and e-way bill details for two B2B invoices.

## 3. Compliance

1. Reconcile purchases with a GSTR-2B you create (include one mismatch and one supplier non-filer).
2. Generate GSTR-1; resolve uncertain transactions; export JSON.
3. Prepare GSTR-3B; compute set-off in the correct order; record the set-off journal and the payment voucher (including RCM paid in cash).
4. Produce Receivables ageing and branch-wise profitability.

## Deliverable checklist

| Item | Done? |
|---|---|
| Company + GST masters complete | |
| Purchases, sales, notes recorded | |
| RCM entries and self-invoices | |
| E-invoice/e-way bill details | |
| GSTR-2B reconciliation with actions | |
| GSTR-1 JSON + GSTR-3B with set-off | |
| Payment vouchers, receivables ageing, branch P&L | |

## How It Actually Works

A GST month is a closed loop: every sale and purchase recorded with correct masters feeds the returns, the returns determine tax payable, reconciliation verifies credits against the portal, and payment entries bring the books back in line with the government's ledgers. When the loop is run carefully each month, annual returns and audits become routine — when it isn't, errors compound into notices, interest and lost credits.

## Exercise

Complete the month for Krishna Electricals and write a one-page compliance summary: output tax, eligible ITC, ITC held back (and why), RCM paid, cash tax paid by head (CGST/SGST/IGST), GSTR-1 and GSTR-3B status, and three issues to resolve before next month.
