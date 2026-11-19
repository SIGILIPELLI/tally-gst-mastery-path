---
description: "Banking: Cheques, e-Payments & Post-Dated Cheques — TallyPrime includes banking utilities that save time and reduce errors: cheque printing, cheque…"
---

# 06 · Banking: Cheques, e-Payments & Post-Dated Cheques

TallyPrime includes banking utilities that save time and reduce errors: cheque printing, cheque registers, e-payment files, post-dated cheque management and deposit slips. This module covers the ones most businesses use.

## 1. Cheque printing and register

1. Enable **cheque printing** in the bank ledger (Set cheque books: Yes; cheque range; cheque printing configuration for your bank's format).
2. TallyPrime provides formats for many Indian banks; adjust dimensions in **Cheque Printing Configuration** if needed.
3. In a Payment voucher from that bank, choose transaction type **Cheque** — TallyPrime picks the next cheque number and prints the cheque with amount in words.
4. **Cheque Register** (Alt+G → Cheque Register) shows issued, blank, cancelled and unused cheques; mark cancelled cheques with reasons.
5. **Cheque Management** tracks cheques deposited and their clearing status.

## 2. e-Payments

1. Enable **e-Payments** in the bank ledger (supported banks) and fill beneficiary bank details (account number, IFSC) in party ledgers.
2. Record Payment vouchers with transaction type **e-Fund Transfer** (NEFT/RTGS/IMPS).
3. Open **Banking → e-Payments** report, select payments and **export the bank-specific payment file** for upload on your net banking portal (or use direct connected banking where supported).
4. After the bank processes payments, update the status and UTR numbers; the entries flow into bank reconciliation.
5. Apply maker-checker controls: one person creates, another approves uploads in net banking.

## 3. Post-dated cheques (PDCs)

1. A PDC is a cheque dated in the future — common for rent, EMIs and customer instalments.
2. In TallyPrime, record the voucher with the future date and mark it **Post-Dated** (voucher setting); it doesn't affect balances until that date.
3. **Post-Dated Summary** (Alt+G → Post-Dated Vouchers) lists upcoming receipts and payments — useful for cash flow forecasting.
4. On the due date, the voucher becomes regular automatically; deposit or present the cheque and reconcile.

## 4. Deposit slips and payment advice

1. **Deposit Slip** report generates a list of cheques/cash to deposit — print and take to the bank.
2. **Payment Advice** sends parties details of payments made (invoices settled, TDS deducted).
3. Email advice directly with **Alt+M**.

## 5. Dishonoured cheques

1. If a customer's cheque bounces, record a reversal: Dr Customer / Cr Bank, plus bank charges (Dr Bank Charges / Cr Bank) and optionally recover charges from the customer.
2. Mark the original cheque as dishonoured in cheque management for tracking.
3. Note legal timelines under the Negotiable Instruments Act if you plan to act on a dishonoured cheque.

## Cheat sheet

| Utility | Purpose |
|---|---|
| Cheque printing | Print cheques from payment vouchers |
| Cheque Register | Track cheque numbers and status |
| e-Payments | Export NEFT/RTGS bank files |
| Post-Dated Summary | Upcoming cheques for cash planning |
| Deposit Slip | Bank deposit list |
| Payment Advice | Inform parties of payments |

## How It Actually Works

Banking utilities read the same payment and receipt vouchers that drive your books, adding instrument details (cheque numbers, UTRs, dates) that the bank also records. Because both sides share identifiers, reconciliation becomes largely automatic. Post-dated vouchers sit outside current balances until their date, giving you a forward view of committed cash flows without distorting today's books.

## Exercise

Configure cheque printing for your bank ledger, issue two cheque payments and cancel one cheque. Record three NEFT supplier payments and generate the e-payment file. Record two post-dated receipts from customers, view the Post-Dated Summary, and record one dishonoured cheque with bank charges.
