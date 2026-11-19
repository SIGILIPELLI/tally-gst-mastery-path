---
description: "Payment, Receipt, Contra & Journal Vouchers — A voucher is how you record a transaction in TallyPrime. This module covers the four core accounting…"
---

# 04 · Payment, Receipt, Contra & Journal Vouchers

A **voucher** is how you record a transaction in TallyPrime. This module covers the four core accounting vouchers you'll use for nearly all non-trading transactions.

## 1. Voucher basics

1. Open vouchers with **Alt+G → Vouchers** (or Gateway → Vouchers), then pick the type with function keys: **F4 Contra**, **F5 Payment**, **F6 Receipt**, **F7 Journal**, **F8 Sales**, **F9 Purchase**.
2. Change the date with **F2** (in Educational Mode use 1st, 2nd or 31st).
3. TallyPrime offers **single-entry mode** (Account at top, particulars below) or **double-entry mode** (Dr/Cr lines). Toggle via **F12 → Use single entry mode for Payment/Receipt/Contra**.
4. Always write a **narration** explaining the transaction — auditors and your future self will thank you.

## 2. Payment voucher (F5) — money going out

1. Paid rent ₹15,000 from HDFC Bank: Account = HDFC Bank; Particulars = Rent ₹15,000.
2. Paid Lakshmi Paper Mart ₹50,000 by NEFT: Account = HDFC Bank; Particulars = Lakshmi Paper Mart ₹50,000.
3. Paid electricity ₹3,200 in cash: Account = Cash; Particulars = Electricity ₹3,200.
4. TallyPrime warns if cash would go negative — a useful control.

## 3. Receipt voucher (F6) — money coming in

1. Received ₹30,000 from Vijay Book Stall by UPI: Account = HDFC Bank; Particulars = Vijay Book Stall ₹30,000.
2. Received commission ₹4,000 in cash: Account = Cash; Particulars = Commission Received (Indirect Incomes) ₹4,000.
3. Bank receipts can capture transaction type (UPI, NEFT, cheque) and instrument details — useful for bank reconciliation.

## 4. Contra (F4) and Journal (F7)

1. **Contra** records transfers between cash and bank accounts only:
   - Deposited cash ₹40,000 into HDFC Bank: Account = HDFC Bank; Particulars = Cash ₹40,000.
   - Withdrew ₹10,000 cash from bank for office use: Account = Cash; Particulars = HDFC Bank ₹10,000.
2. **Journal** records adjustments that don't involve cash or bank:
   - Depreciation on computer ₹4,500: Dr Depreciation (Indirect Expenses) / Cr Computer.
   - Goods worth ₹2,000 taken by owner for personal use: Dr Drawings (Capital Account) / Cr Purchases.
   - Outstanding salary ₹25,000 at month end: Dr Salary / Cr Salary Payable (Current Liabilities).
3. Rule of thumb: **cash/bank involved → Payment, Receipt or Contra; not involved → Journal** (credit sales/purchases use Sales/Purchase vouchers, next module).

## 5. Edit, delete and duplicate

1. Find vouchers in the **Day Book** (Alt+G → Day Book). Select and press Enter to alter.
2. **Alt+D** deletes; **Alt+X** cancels (keeps the voucher number with zero value for audit continuity); **Alt+2** duplicates a voucher.

## Cheat sheet

| Voucher | Key | Use |
|---|---|---|
| Contra | F4 | Cash ↔ bank, bank ↔ bank |
| Payment | F5 | Money out (cash/bank) |
| Receipt | F6 | Money in (cash/bank) |
| Journal | F7 | Non-cash adjustments |
| Delete / Cancel / Duplicate | Alt+D / Alt+X / Alt+2 | |

## How It Actually Works

Voucher types are templates that enforce the right accounts: Payment and Receipt require a cash or bank ledger on one side, Contra allows only cash and bank ledgers, and Journal excludes them by default. Each saved voucher posts debit and credit amounts to the ledgers instantly and updates every report. Voucher numbering per type, with cancellations preserved, creates the continuous audit trail that statutory auditors and GST officers expect.

## Exercise

Record these vouchers for Sri Sai Traders (use allowed dates): rent ₹15,000 by bank; electricity ₹3,200 cash; receipt ₹30,000 from Vijay by UPI; commission received ₹4,000 cash; deposit ₹40,000 cash into bank; depreciation ₹4,500 on the computer; outstanding salary ₹25,000. Then open the Day Book and the Cash and HDFC Bank ledgers to check balances.
