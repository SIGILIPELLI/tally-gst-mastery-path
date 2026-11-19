---
description: "Ledgers & Groups — In TallyPrime, every account is a ledger, and every ledger belongs to a group. The group decides where the ledger appears — Balance…"
---

# 03 · Ledgers & Groups

In TallyPrime, every account is a **ledger**, and every ledger belongs to a **group**. The group decides where the ledger appears — Balance Sheet or Profit & Loss — and how it behaves. Getting groups right is the single most important setup step.

## 1. Predefined groups

1. TallyPrime ships with 28 groups: 15 **primary** groups and 13 **sub-groups**.
2. Balance Sheet primary groups: **Capital Account**, **Loans (Liability)**, **Current Liabilities**, **Fixed Assets**, **Investments**, **Current Assets**, **Branch / Divisions**, **Misc. Expenses (Asset)**, **Suspense A/c**.
3. Profit & Loss primary groups: **Sales Accounts**, **Purchase Accounts**, **Direct Incomes**, **Indirect Incomes**, **Direct Expenses**, **Indirect Expenses**.
4. Useful sub-groups: **Bank Accounts**, **Bank OD A/c**, **Cash-in-Hand**, **Sundry Debtors**, **Sundry Creditors**, **Duties & Taxes**, **Provisions**, **Reserves & Surplus**, **Secured Loans**, **Unsecured Loans**, **Loans & Advances (Asset)**, **Deposits (Asset)**, **Stock-in-Hand**.
5. Two ledgers exist by default: **Cash** (under Cash-in-Hand) and **Profit & Loss A/c**.

## 2. Create ledgers

1. **Alt+G → Create Master → Ledger** (or Gateway → Create → Ledger).
2. Example ledgers for Sri Sai Traders:

| Ledger | Group | Opening balance |
|---|---|---|
| Capital – Srinivas | Capital Account | 5,00,000 Cr |
| HDFC Bank | Bank Accounts | 3,00,000 Dr |
| Vijay Book Stall | Sundry Debtors | 20,000 Dr |
| Lakshmi Paper Mart | Sundry Creditors | 0 |
| Rent | Indirect Expenses | — |
| Freight Inward | Direct Expenses | — |
| Sales | Sales Accounts | — |
| Purchases | Purchase Accounts | — |

3. For debtors/creditors, fill **mailing details**, state, and later GST registration details and **bill-wise** settings.
4. For bank ledgers, add account number, IFSC and branch (used for cheque printing and e-payments later).
5. Press **Ctrl+A** to save each.

## 3. Direct vs indirect

1. **Direct expenses/incomes** relate to buying or making goods: freight inward, carriage, wages in a factory. They affect **gross profit**.
2. **Indirect expenses/incomes** are running costs and other income: rent, salaries (office), advertising, interest received. They affect **net profit**.
3. Misclassifying freight inward as indirect overstates gross profit — a common error.

## 4. Custom groups and alteration

1. Create your own groups for clearer reports: e.g. "Marketing Expenses" under Indirect Expenses, "Hyderabad Debtors" under Sundry Debtors.
2. **Alter** a ledger via **Alt+G → Alter Master → Ledger**; changing its group moves all its history to the new place in reports.
3. **Chart of Accounts** (**Alt+G → Chart of Accounts**) shows the full group-ledger tree.
4. Use **Multi-ledger creation** (Alt+G → Create Master → Multi Ledger) to create many ledgers under one group quickly.

## Cheat sheet

| Ledger | Correct group |
|---|---|
| Owner's investment | Capital Account |
| Bank account | Bank Accounts |
| Customer | Sundry Debtors |
| Supplier | Sundry Creditors |
| GST/TDS payable | Duties & Taxes |
| Office rent, salary | Indirect Expenses |
| Freight inward, factory wages | Direct Expenses |
| Furniture, computer | Fixed Assets |

## How It Actually Works

Groups encode accounting classification once, so every voucher posted to a ledger automatically flows to the right report section. The Balance Sheet is simply the closing balances of all Balance Sheet groups at a date; the P&L aggregates the income and expense groups for a period, splitting direct items above gross profit and indirect items below it. That's why a single wrong group silently distorts every report that uses it.

## Exercise

Create all eight ledgers in the table with opening balances, plus: "Electricity" (Indirect Expenses), "Computer" (Fixed Assets), "Unsecured Loan – Friend" (Unsecured Loans) and two more customers and suppliers. Open the Chart of Accounts and the opening Trial Balance (Alt+G → Trial Balance) — check that the Difference in Opening Balances is explained by your entries.
