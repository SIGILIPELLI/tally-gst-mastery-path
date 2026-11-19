---
description: "TDS: Deduction, Payment & Returns — Tax Deducted at Source (TDS) requires a payer to deduct income tax from certain payments — contractor bills,…"
---

# 01 · TDS: Deduction, Payment & Returns

**Tax Deducted at Source (TDS)** requires a payer to deduct income tax from certain payments — contractor bills, professional fees, rent, commission, salaries — and deposit it with the government. This module covers the main rules and recording TDS in TallyPrime.

> **2026 note:** From 1 April 2026 the **Income-tax Act, 2025** replaced the Income-tax Act, 1961. TDS provisions are consolidated (largely in section 393) with new form numbers, while most rates and thresholds carried over. Many professionals — and many software screens — still refer to the familiar 1961-Act labels (194C, 194J…), which this lesson shows for clarity. Always confirm current rates, thresholds and forms on **incometax.gov.in** and in your TallyPrime release notes.

## 1. Common TDS categories (familiar labels)

| Nature of payment | Familiar section | Rate (resident) | Threshold (indicative) |
|---|---|---|---|
| Contractors | 194C | 1% individual/HUF, 2% others | ₹30,000 single / ₹1,00,000 in a year |
| Professional fees | 194J | 10% | ₹50,000 in a year |
| Technical services, royalty (certain) | 194J | 2% | ₹50,000 in a year |
| Rent – land/building/furniture | 194I | 10% | ₹50,000 per month |
| Rent – plant/machinery | 194I | 2% | ₹50,000 per month |
| Commission/brokerage | 194H | 2% | ₹20,000 in a year |
| Purchase of goods (large buyers) | 194Q | 0.1% above ₹50 lakh | Buyer turnover > ₹10 crore |
| Salaries | 192 | Slab rates | Above exemption |

1. If the payee doesn't provide a valid **PAN**, TDS generally applies at a higher rate (often 20%).
2. Deduct at the time of credit to the payee's account or payment, whichever is earlier.

## 2. Deposit, returns and certificates

1. Deposit TDS by the **7th of the following month** (for March, by **30 April**) through the challan on the income tax portal.
2. File quarterly TDS statements (salary and non-salary; separate statements for non-residents) by **31 July, 31 October, 31 January and 31 May**.
3. Issue TDS certificates to payees (quarterly for non-salary, annually for salary employees) from the TRACES portal.
4. Interest applies on late deduction/deposit and fees on late statements.
5. You need a **TAN** (Tax Deduction Account Number) to deduct TDS.

## 3. TDS in TallyPrime

1. **F11 → Enable Tax Deducted at Source (TDS)**; enter TAN, deductor type and responsible person details.
2. Create TDS **nature of payment** masters (TallyPrime includes standard ones) with rates and thresholds.
3. Create a **TDS payable** ledger under Duties & Taxes (Type: TDS), linked to the nature of payment.
4. In party ledgers (e.g. "Sharma Contractors"), set **Is TDS deductable: Yes**, deductee type (Individual/Company) and PAN.
5. In expense ledgers (e.g. "Contract Charges"), set TDS applicable with the nature of payment.

## 4. Worked example

1. Contractor bill ₹1,20,000 (company contractor, 2%): **Journal** or **Purchase** voucher — Dr Contract Charges ₹1,20,000; Cr Sharma Contractors ₹1,17,600; Cr TDS Payable – Contractors ₹2,400. TallyPrime calculates the TDS once thresholds are crossed.
2. Pay the contractor ₹1,17,600 (Payment voucher).
3. Deposit TDS ₹2,400 by the 7th: **Payment** voucher using **Stat Payment** (Ctrl+F) to fill period and nature of payment, then record the challan details (BSR code, challan number, date).
4. Generate TDS reports: **Alt+G → TDS Reports** — computation, challan reconciliation, return forms (export for the return preparation utility).

## Cheat sheet

| Step | Rule |
|---|---|
| Deduct | At credit or payment, whichever earlier |
| No PAN | Higher rate |
| Deposit | 7th of next month (30 April for March) |
| Returns | Quarterly: 31 Jul, 31 Oct, 31 Jan, 31 May |
| Certificates | From TRACES |
| TallyPrime | F11 TDS, nature of payment, party PAN, Stat Payment |

## How It Actually Works

TDS collects tax progressively at the point income is paid, rather than waiting for the recipient's annual return. The deductor acts as a collection agent: amounts deducted are linked to the payee's PAN through quarterly statements, appear in the payee's tax credit statement, and are credited against their final tax liability. That's why accurate PANs, correct categories and timely statements matter — errors leave payees without credit and expose the deductor to interest, fees and disallowance of the expense.

## Exercise

For a manufacturing company, record: a contractor bill ₹1,20,000 (company, 2%), professional fees ₹75,000 to a CA, monthly office rent ₹80,000, and commission ₹25,000 to an agent without PAN. Calculate TDS for each, record vouchers and the deposit, and list the due date for deposit and for the quarterly statement.
