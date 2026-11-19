---
description: "Payroll: Salary, PF & ESI — TallyPrime has a built-in payroll module that calculates salaries, statutory deductions and generates payslips and compliance…"
---

# 03 · Payroll: Salary, PF & ESI

TallyPrime has a built-in payroll module that calculates salaries, statutory deductions and generates payslips and compliance reports. This module sets up payroll for a small company. Statutory rates are as of 2026; the new **labour codes** (in force from November 2025, with rules being notified) may change wage definitions and contributions — confirm with current EPFO/ESIC notifications.

## 1. Statutory basics

1. **Provident Fund (EPF)**: applies to establishments with 20+ employees (voluntary below). Employee contributes **12%** of basic + DA; employer contributes **12%**, of which **8.33%** (capped on ₹15,000 wages = ₹1,250/month) goes to the **pension scheme (EPS)** and the rest to EPF. Employer also pays admin charges (0.5%) and EDLI (0.5%). Mandatory coverage for wages up to ₹15,000 (higher-wage employees can be covered).
2. **ESI**: applies to establishments with 10+ employees (in notified areas) for employees earning up to **₹21,000** a month. Employee **0.75%**, employer **3.25%** of gross wages.
3. **Professional tax**: state-specific (e.g. Maharashtra up to ₹200/month with ₹300 in February; Karnataka ₹200 for salaries above a threshold); some states don't levy it.
4. **TDS on salary**: deducted monthly based on estimated annual tax under the regime the employee chooses (the new regime is the default).
5. **Labour Welfare Fund** and **gratuity/bonus** obligations may also apply.

## 2. Payroll setup in TallyPrime

1. **F11 → Maintain Payroll: Yes**; enable statutory features (PF, ESI, PT, Income Tax) and enter registration numbers.
2. Create **employee groups** (Office, Sales, Factory) and **employees** with joining date, designation, PAN, UAN, ESI number, bank account.
3. Create **attendance/production types**: Present, Absent, Leave, Overtime hours.
4. Create **pay heads**: Basic (earnings, on attendance), HRA (% of basic), Conveyance (flat), Special Allowance, Overtime (rate per hour), PF Employee (deduction), ESI Employee, Professional Tax, TDS on Salary; employer contributions PF and ESI.
5. Define **salary details** for each employee or group with effective dates.

## 3. Monthly processing

1. Record **Attendance voucher** (Ctrl+F5) — days present, leave, overtime.
2. Process the **Payroll voucher** (Ctrl+F4 → Payroll Auto Fill): TallyPrime calculates earnings, deductions and net pay.
3. Example — Priya, basic ₹14,000, HRA ₹5,600, special ₹2,400 (gross ₹22,000):
   - PF employee 12% × 14,000 = ₹1,680; employer ₹1,680 (EPS ₹1,166, EPF ₹514).
   - ESI not applicable (gross above ₹21,000).
   - Professional tax ₹200 → net pay ₹20,120 (before any TDS).
4. Record the **salary payment** (Payment voucher or bank transfer file) and the **employer contribution** journal.
5. Pay PF and ESI by the **15th** of the following month (ECR filing on the EPFO portal; ESI on the ESIC portal).

## 4. Payroll reports

1. **Payslips** (print/email), **Pay Sheet**, **Attendance Sheet**, **Payment Advice** for the bank.
2. Statutory reports: PF ECR, ESI monthly contribution, PT computation, Form 16 data for TDS.
3. Gratuity computation and leave encashment reports where configured.

## Cheat sheet

| Item | Rule (2026) |
|---|---|
| PF | 12% employee + 12% employer (8.33% EPS capped at ₹1,250) |
| PF wage ceiling | ₹15,000 (mandatory) |
| ESI | 0.75% employee + 3.25% employer, wages ≤ ₹21,000 |
| PF/ESI due | 15th of next month |
| Payroll voucher | Ctrl+F4 |
| Attendance | Ctrl+F5 |

## How It Actually Works

Payroll in TallyPrime separates **what** each employee earns (salary structure built from pay heads with formulas) from **how much** they worked (attendance), then computes statutory deductions using configured rules and ceilings. Payroll vouchers post directly to salary expense, liability and statutory payable ledgers, so payroll costs flow into the P&L and the statutory dues sit as liabilities until paid — making compliance due dates visible in the books.

## Exercise

Set up payroll for five employees with different salaries (two below ₹21,000 gross for ESI). Create pay heads with formulas, record one month's attendance, process payroll, and generate payslips, the pay sheet and PF/ESI reports. Calculate the total employer cost for the month.
