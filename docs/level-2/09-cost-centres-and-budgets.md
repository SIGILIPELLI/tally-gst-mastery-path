---
description: "Cost Centres & Budgets — Total profit tells you how the business did; cost centres tell you which branch, department, project or salesperson drove it.…"
---

# 09 · Cost Centres & Budgets

Total profit tells you how the business did; **cost centres** tell you which branch, department, project or salesperson drove it. **Budgets** let you plan and compare actual results. This module sets up both.

## 1. Cost categories and centres

1. **F11 → Maintain Cost Centres: Yes**; enable **Cost Categories** if you need more than one dimension.
2. **Cost category** = a dimension: "Branches", "Salespeople", "Projects".
3. **Cost centres** under each: Branches → Vijayawada, Guntur, Rajahmundry; Salespeople → Ravi, Kiran.
4. Create via **Alt+G → Create Master → Cost Category / Cost Centre**.

## 2. Allocate in vouchers

1. In ledgers you want to analyse (Sales, Rent, Salary, Freight, Advertising), set **Cost centres are applicable: Yes**.
2. While entering a voucher, TallyPrime asks for allocation: e.g. Rent ₹45,000 → Vijayawada ₹25,000, Guntur ₹12,000, Rajahmundry ₹8,000.
3. Sales can be allocated by branch and by salesperson in the same voucher (different categories).
4. Use **cost centre classes** to apply a fixed allocation automatically (e.g. salary always split 50/30/20).

## 3. Cost centre reports

1. **Alt+G → Cost Centre Break-up**, **Category Summary** and **Ledger break-up**.
2. Branch profitability: allocate sales and direct/indirect costs by branch to see each branch's contribution.
3. Salesperson performance: sales value, margin and discounts by person.
4. Drill down to vouchers to verify allocations.

## 4. Budgets

1. **F11 → Maintain Budgets** (Budgets and Controls in some releases), then **Alt+G → Create Master → Budget**.
2. Name ("FY 2026-27 Plan"), period (1-4-2026 to 31-3-2027), and set budget amounts on **groups**, **ledgers** or **cost centres**: e.g. Indirect Expenses ₹18,00,000 for the year; Advertising ₹2,40,000; Sales target ₹3,00,00,000; Guntur branch expenses ₹4,00,000.
3. Budget type: **On closing balance**, **on nett transactions** — choose net transactions for income/expense period totals.
4. Compare in **Trial Balance**, **Group Summary** or **Cost Centre** reports by adding the budget column (**F12** / Budget Variance): actual vs budget with variance and percentage.
5. Review monthly; investigate variances above a threshold (e.g. ±10%).

## Cheat sheet

| Feature | Path |
|---|---|
| Enable | F11 → Cost Centres / Budgets |
| Category | Dimension (branch, person, project) |
| Allocation | In voucher, ledgers with cost centres applicable |
| Classes | Auto-allocation rules |
| Reports | Cost Centre Break-up, Category Summary |
| Budget | Create Master → Budget; variance in reports |

## How It Actually Works

Cost centres add extra dimensions to each posting without changing the accounts: the same rent entry still hits the Rent ledger, but also carries tags for the branch it belongs to. Reports then slice the general ledger by those tags. Budgets are stored targets attached to groups, ledgers or centres for a period; variance reports subtract budget from actual, turning the books into a management tool that highlights where performance departs from plan.

## Exercise

Set up branch and salesperson cost categories for Godavari Wholesale Mart. Record five sales and four expenses with allocations, then produce branch-wise profitability. Create an annual budget for sales, advertising and rent by branch, and generate a budget variance report for the month.
