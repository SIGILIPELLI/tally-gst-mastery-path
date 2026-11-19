---
description: "GST Setup in TallyPrime — With GST concepts in place, this module configures TallyPrime to calculate, record and report GST automatically. Our Level 2…"
---

# 01 · GST Setup in TallyPrime

With GST concepts in place, this module configures TallyPrime to calculate, record and report GST automatically. Our Level 2 practice company is *Godavari Wholesale Mart*, a registered regular taxpayer in Vijayawada, Andhra Pradesh, trading in household goods.

## 1. Enable GST for the company

1. Press **F11 (Company Features)** and set **Enable Goods and Services Tax (GST)** to **Yes**.
2. In the GST details (or **Alt+K → GST → Show More** in recent releases): State **Andhra Pradesh**, Registration type **Regular**, **GSTIN** (e.g. `37ABCDE1234F1Z9` — 37 is Andhra Pradesh), Applicable from 1-4-2026.
3. Set **Periodicity of GSTR-1**: Monthly (or Quarterly if you've opted for QRMP).
4. Enable options as relevant: e-Way Bill applicable (and threshold), e-Invoicing applicable (if your aggregate turnover requires it — Module 6), and Tax Liability on Advance Receipts.
5. Save with **Ctrl+A**.

## 2. Tax ledgers

1. Create under group **Duties & Taxes**, **Type of duty/tax: GST**, with the matching **Tax type**:

| Ledger | Tax type |
|---|---|
| Output CGST | Central Tax |
| Output SGST | State Tax |
| Output IGST | Integrated Tax |
| Input CGST | Central Tax |
| Input SGST | State Tax |
| Input IGST | Integrated Tax |

2. Some businesses use single CGST/SGST/IGST ledgers for both input and output; separate ledgers make reconciliation clearer.
3. Leave the percentage blank on tax ledgers so TallyPrime picks the rate from item or ledger GST details.

## 3. Sales and purchase ledgers

1. Alter **Sales** and **Purchases** ledgers: **GST applicability: Applicable**, set **Nature of transaction** if needed (e.g. "Sales Taxable" — TallyPrime decides intra/inter-state from the party's state).
2. Create separate ledgers if you have distinct types: **Sales – Exempt**, **Sales – Exports**, **Purchases – Imports**.
3. GST rates are best set on **stock items** (next section), with ledgers left to inherit them.

## 4. Party and item GST details

1. For each customer/supplier ledger: **Registration type** (Regular, Composition, Unregistered/Consumer, SEZ, Overseas), **GSTIN/UIN**, **State**, and address. TallyPrime validates GSTIN format.
2. For each **stock item** (or stock group): **HSN/SAC** code and description, **Taxability** (Taxable, Exempt, Nil-rated), **GST rate** (e.g. 18% → CGST 9% / SGST 9% / IGST 18% shown automatically), and **Type of supply** (Goods/Services).
3. Use **stock group** level GST details when many items share the same HSN and rate — items inherit them.
4. For services, create service ledgers (e.g. "Repair Services Income") with SAC and rate.
5. TallyPrime's **GST Rate Setup** screen lets you review and update rates for many items at once.

## Cheat sheet

| Setting | Where |
|---|---|
| Enable GST, GSTIN, state, periodicity | F11 / Alt+K → GST |
| Tax ledgers | Duties & Taxes, Type = GST, Tax type |
| Sales/Purchase ledger | GST applicable |
| Party details | Registration type, GSTIN, state |
| Item details | HSN/SAC, taxability, rate |
| Bulk rate review | GST Rate Setup |

## How It Actually Works

TallyPrime decides GST on each invoice by combining three facts: your company's state, the party's state (or place of supply), and the item's taxability and rate. Same state → CGST and SGST at half the rate each; different state → IGST at the full rate. Because rates live in masters (items, groups or ledgers) with effective dates, a rate change can be applied from a specific date without touching old invoices — critical after events like the 2025 rate rationalisation.

## Exercise

Create Godavari Wholesale Mart with GST enabled (monthly GSTR-1). Create the six tax ledgers, GST-applicable Sales and Purchases ledgers, three customers (one in Andhra Pradesh, one in Telangana, one unregistered consumer) and two suppliers with GSTINs, and five stock items with HSN codes and current rates (look up actual rates for items such as steel utensils, LED bulbs, plastic buckets, detergent and pressure cookers on the CBIC rate finder).
