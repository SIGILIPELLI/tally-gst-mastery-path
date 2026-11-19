---
description: "Internal Controls, Security & the Edit Log — Accounting data is valuable and sensitive. Weak controls lead to errors, fraud and failed audits. This module…"
---

# 03 · Internal Controls, Security & the Edit Log

Accounting data is valuable and sensitive. Weak controls lead to errors, fraud and failed audits. This module sets up user security, access rights, period locks and TallyPrime's **edit log** — which also helps meet the Companies Act requirement for an audit trail.

## 1. Why controls matter

1. **Segregation of duties**: the person who records purchases shouldn't approve payments or reconcile the bank.
2. **Authorisation**: payments above a limit need approval.
3. **Reconciliation**: bank, GST, receivables, payables and stock reconciled regularly.
4. **Audit trail**: a record of who changed what and when.
5. Under the Companies (Accounts) Rules, companies must use accounting software with an **audit trail (edit log)** that can't be disabled, retained for the statutory period.

## 2. Users and security in TallyPrime

1. **Alt+K → Security Control / Users and Passwords** (or Company → Security): enable security and create an **administrator** (owner) with a strong password.
2. Define **security levels / roles**: Data Entry (create vouchers only), Accountant (create, alter, view reports), Auditor (view only), Owner (full).
3. Restrict access by voucher type, reports, and features (e.g. data entry can't view P&L or alter masters).
4. Create **users** with their role; enforce password changes; remove access promptly when people leave.
5. Enable **TallyVault** encryption for sensitive data, and keep the vault password secure — it can't be recovered.

## 3. Edit log and period locks

1. In recent TallyPrime releases, enable **Edit Log** (for companies it's expected to be on; TallyPrime offers an Edit Log edition/mode where it can't be disabled).
2. The edit log records creation, alteration and deletion of vouchers and masters with user, date and time, and previous versions.
3. View it from the voucher (**Related Reports → Edit Log**) or the Edit Log reports for the company.
4. **Lock periods** after closing (e.g. lock entries up to 31 March after audit) so no one alters closed periods; changes require administrator unlock and leave a trace.
5. Restrict **back-dated entries** beyond a number of days for data entry users.

## 4. Practical control checklist

1. Daily: review Day Book for unusual entries; cash count matches books.
2. Weekly: bank reconciliation; approval of payment batches; review cancelled/deleted vouchers in the edit log.
3. Monthly: GST and TDS reconciliation; receivables/payables review; stock count samples; MIS review by owner.
4. Annually: full stock verification, balance confirmations, fixed asset verification, access review.
5. Keep supporting documents (scans attached or referenced in narrations).

## Cheat sheet

| Control | TallyPrime feature |
|---|---|
| Access | Users, roles, security levels |
| Encryption | TallyVault |
| Audit trail | Edit Log |
| Closed periods | Lock period / restrict back-dating |
| Review | Day Book, edit log reports |
| Segregation | Separate roles for entry, approval, reconciliation |

## How It Actually Works

Controls work by making errors and fraud either impossible (access restrictions, locks) or visible (edit logs, reconciliations, reviews). An audit trail changes behaviour: when every alteration is recorded with the user's identity and the original values, quietly manipulating records stops being practical. Auditors rely on these controls to decide how much detailed testing they need — strong controls mean faster, cheaper audits.

## Exercise

Set up security for a company: an owner, an accountant, a data entry operator and an auditor, each with appropriate rights. Enable the edit log, make and alter a voucher as the data entry user, then review the change history as the owner. Write a one-page control checklist for a 10-person business.
