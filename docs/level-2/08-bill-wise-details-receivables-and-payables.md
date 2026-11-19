---
description: "Bill-wise Details: Receivables & Payables — Knowing that customers owe ₹4 lakh in total isn't enough — you need to know which invoices are unpaid, how old…"
---

# 08 · Bill-wise Details: Receivables & Payables

Knowing that customers owe ₹4 lakh in total isn't enough — you need to know **which invoices** are unpaid, **how old** they are, and **who to chase**. Bill-wise accounting in TallyPrime tracks every invoice and payment against it.

## 1. Enable and configure

1. **F11 → Maintain Bill-wise details: Yes** (and for non-trading accounts if you track loans or advances bill-wise).
2. In each customer/supplier ledger, set **Maintain balances bill-by-bill: Yes** and a **Default credit period** (e.g. 30 days).
3. Opening balances can be broken into individual bills with dates.

## 2. Reference types

1. **New Ref** — a new bill (each sales or purchase invoice).
2. **Agst Ref** — payment or receipt against an existing bill.
3. **Advance** — money received/paid before the invoice.
4. **On Account** — payment not linked to a specific bill (use sparingly; reconcile later).
5. When recording a receipt, TallyPrime shows pending bills — choose the bills being paid.

## 3. Worked example

1. Sale to Srinivasa Stores: Inv. GWM/060, ₹59,000, credit 30 days (New Ref).
2. Sale: Inv. GWM/072, ₹35,400 (New Ref).
3. Receipt ₹70,000 by NEFT: Agst Ref GWM/060 ₹59,000 and Agst Ref GWM/072 ₹11,000 → GWM/072 has ₹24,400 pending.
4. Advance ₹20,000 from a new customer for an upcoming order (Advance) — later adjusted against the invoice. Note: GST on advances for services is payable when received; for goods, generally not.

## 4. Outstanding and ageing reports

1. **Alt+G → Receivables** (Bills Receivable) and **Payables**: pending bills with due dates and overdue days.
2. **Ledger outstanding**: one party's pending bills — share as a statement.
3. **Ageing analysis** (F6/configure periods): 0–30, 31–60, 61–90, 90+ days — identify risky debts.
4. **Interest calculation** can be configured for overdue bills (F11 → Activate Interest Calculation) and applied per party.
5. **Reminder letters**: print or email outstanding statements and reminders to customers.

## 5. Using it in practice

1. Weekly collection list: top overdue customers, amounts, last contact.
2. Supplier payment planning: pay by due date to keep credit terms (and meet GST's 180-day rule for ITC).
3. Watch **days sales outstanding (DSO)** = receivables ÷ credit sales × days; rising DSO strains cash.

## Cheat sheet

| Concept | Use |
|---|---|
| New Ref | New invoice |
| Agst Ref | Payment against a bill |
| Advance | Paid/received before invoice |
| On Account | Unlinked (reconcile later) |
| Receivables / Payables | Pending bills, overdue days |
| Ageing | 0–30 / 31–60 / 61–90 / 90+ |
| DSO | Receivables ÷ credit sales × days |

## How It Actually Works

Without bill-wise tracking, a party ledger is just a running balance — payments can't be matched to invoices, so ageing and disputes become guesswork. Bill references create a link between each invoice and the receipts settling it, which lets TallyPrime compute exactly what's overdue and by how long. That information drives collections, credit decisions and compliance rules like the 180-day ITC condition on supplier payments.

## Exercise

Enable bill-wise details for Godavari Wholesale Mart. Record six invoices across three customers, two partial receipts with Agst Ref, one advance and one on-account receipt. Produce the Receivables and ageing reports, print one customer's outstanding statement and calculate DSO for the month.
