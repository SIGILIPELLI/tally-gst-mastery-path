---
description: "Bank Reconciliation — Your books and the bank statement rarely match on any given day — cheques take time to clear, banks deduct charges you haven't…"
---

# 07 · Bank Reconciliation

Your books and the bank statement rarely match on any given day — cheques take time to clear, banks deduct charges you haven't recorded, customers pay directly into your account. **Bank reconciliation** explains every difference and catches errors or fraud early.

## 1. Why differences occur

1. **Cheques issued but not yet presented** — recorded in books, not yet in the bank.
2. **Cheques deposited but not yet cleared** — in books, not yet credited by the bank.
3. **Bank charges, interest, GST on charges** — in the statement, not yet in books.
4. **Direct deposits / UPI collections** you haven't recorded.
5. **Errors** — wrong amount or wrong ledger in books.

## 2. Reconcile in TallyPrime

1. Open the bank ledger: **Alt+G → Bank Reconciliation**, choose **HDFC Bank** (or open the bank ledger and use the Reconcile option).
2. The screen lists vouchers with a **Bank Date** column. For each entry that appears in your bank statement, enter the date the bank processed it.
3. Entries without a bank date remain unreconciled.
4. At the bottom TallyPrime shows **Balance as per Company Books**, **Amounts not reflected in bank**, and **Balance as per Bank**. Compare the last with your statement's closing balance.
5. If they don't match, look for statement entries missing from your books.

## 3. Record missing entries

1. Bank charges ₹590 (₹500 + 18% GST): Payment voucher — Account HDFC Bank; Particulars Bank Charges ₹500 and Input GST (if you claim it) ₹90.
2. Interest credited ₹1,200: Receipt voucher — HDFC Bank / Interest Received (Indirect Incomes).
3. Direct UPI from a customer ₹8,000: Receipt voucher — HDFC Bank / customer ledger.
4. Return to reconciliation and set bank dates for these entries.

## 4. Auto reconciliation and statements

1. TallyPrime supports **importing bank statements** (Excel or supported formats, and connected banking for supported banks) to match entries automatically.
2. Review suggested matches carefully, then accept.
3. Unmatched statement lines become a to-do list of vouchers to create.
4. Reconcile at least **monthly**, ideally weekly for active accounts.

## Worked example

| Item | Amount (₹) |
|---|---|
| Balance as per books | 2,15,400 Dr |
| Less: cheques deposited not cleared | (18,000) |
| Add: cheques issued not presented | 12,500 |
| Less: bank charges not recorded | (590) |
| Add: interest not recorded | 1,200 |
| **Balance as per bank statement** | **2,10,510** |

## Cheat sheet

| Situation | Action |
|---|---|
| Entry in both books & statement | Set bank date |
| In books, not in statement | Leave unreconciled (timing) |
| In statement, not in books | Create voucher, then reconcile |
| Error in books | Alter voucher |
| Auto match | Import statement, review matches |

## How It Actually Works

Reconciliation compares two independent records of the same account. Timing differences resolve themselves as cheques clear; missing entries and errors don't, and reconciliation is the control that exposes them. In TallyPrime, the bank date doesn't change your accounting date — it only marks when the bank processed the entry, so the books keep the true transaction date while the reconciliation report proves the bank balance.

## Exercise

Using your HDFC Bank ledger, assume a bank statement that shows all your entries except one ₹18,000 cheque deposit and one ₹12,500 cheque issued, plus bank charges ₹590 and interest ₹1,200 not in your books. Record the missing vouchers, set bank dates, and confirm that the "Balance as per Bank" matches the statement.
