---
description: "Core Reports: Day Book, Trial Balance, P&L, Balance Sheet — TallyPrime's value is in its reports — always up to date, with drill-down from totals to…"
---

# 08 · Core Reports: Day Book, Trial Balance, P&L, Balance Sheet

TallyPrime's value is in its reports — always up to date, with drill-down from totals to individual vouchers. This module teaches you to read the essential reports and use them to check your work.

## 1. Day Book

1. **Alt+G → Day Book** lists all vouchers for a date or period (**Alt+F2** to change period).
2. Use it daily to review entries; press Enter on any voucher to open and correct it.
3. Filter by voucher type with **F4** or configure columns with **F12**.

## 2. Ledger and group summaries

1. **Ledger** report (Alt+G → Ledger) shows all entries for one account with running balance — e.g. Vijay Book Stall's account statement.
2. **Group Summary** (e.g. Sundry Debtors) lists all customers with balances — who owes how much.
3. **Cash/Bank Books** show cash and bank movement.

## 3. Trial Balance

1. **Alt+G → Trial Balance** shows closing balances of all groups; press **Alt+F1** (Detailed) or expand groups to see ledgers.
2. Total debits must equal total credits. A "Difference in opening balances" line means opening balances don't agree — fix them in ledger masters.
3. Scan for oddities: a supplier with a debit balance (overpaid?), cash with a credit balance (impossible), expenses in the wrong group.

## 4. Profit & Loss Account

1. **Alt+G → Profit & Loss A/c** for the period.
2. Top section (trading account): Opening stock + Purchases + Direct Expenses vs Sales + Closing stock → **Gross Profit**.
3. Lower section: Gross Profit + Indirect Incomes − Indirect Expenses → **Net Profit**.
4. Example (illustrative one-month figures): Sales ₹1,35,000; Opening stock ₹99,400; Purchases ₹86,000; Freight inward ₹1,500; Closing stock ₹1,08,200 → Cost of goods sold ₹78,700 → Gross profit ₹56,300. Rent ₹15,000, salary ₹25,000, electricity ₹3,200, depreciation ₹4,500, commission received ₹4,000 → Net profit ₹12,600.

## 5. Balance Sheet

1. **Alt+G → Balance Sheet** at a date: Capital and liabilities on one side, assets on the other.
2. Net profit appears under **Profit & Loss A/c** on the liabilities/capital side.
3. Drill down from Current Assets → Sundry Debtors → a customer → vouchers.
4. Use **F12** to show percentages, comparative periods (**Alt+C** to add a column) or vertical format.

## 6. Export and share

1. **Alt+E** exports to Excel, PDF, JSON or XML; **Alt+M** emails or shares; **Alt+P** prints.
2. Save report views with your preferred configuration for repeated use.

## Cheat sheet

| Report | Answers |
|---|---|
| Day Book | What was entered today/this period? |
| Ledger | Full history of one account |
| Group Summary | Balances of all customers/suppliers |
| Trial Balance | Do debits equal credits? Any odd balances? |
| Profit & Loss | Gross and net profit for a period |
| Balance Sheet | Financial position on a date |

## How It Actually Works

All TallyPrime reports are views computed from the same voucher data, filtered by date and grouped by the group hierarchy — nothing is stored separately, so a corrected voucher instantly corrects every report. The P&L summarises income and expense groups over a period, while the Balance Sheet captures balances at a point in time; profit is the bridge between them, flowing from the P&L into capital. Drill-down is how accountants audit: start from a surprising total and follow it to the vouchers behind it.

## Exercise

Open the Trial Balance, P&L and Balance Sheet for Sri Sai Traders after all your Level 1 entries. Check that debits equal credits, identify gross and net profit, and drill down to find the voucher behind one expense. Export the Balance Sheet to Excel and PDF.
