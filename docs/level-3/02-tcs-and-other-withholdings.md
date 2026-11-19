---
description: "TCS & Other Withholdings — While TDS is deducted by the payer, Tax Collected at Source (TCS) is collected by the seller from the buyer on specified…"
---

# 02 · TCS & Other Withholdings

While TDS is deducted by the **payer**, **Tax Collected at Source (TCS)** is collected by the **seller** from the buyer on specified transactions. GST also has its own TCS for e-commerce operators. This module covers both and how to record them. Rules are as of 2026 — confirm current provisions under the Income-tax Act, 2025 and GST law.

## 1. Income-tax TCS — common cases

1. Sale of specified goods: scrap (1%), alcoholic liquor for human consumption (1%), tendu leaves, timber and forest produce, minerals (coal, lignite, iron ore) at notified rates.
2. Sale of a **motor vehicle** above ₹10 lakh (1%), and from 2025 certain notified luxury goods above ₹10 lakh.
3. **Foreign remittances under LRS** and overseas tour packages: TCS above thresholds (e.g. 20% on certain LRS remittances above ₹10 lakh; lower or nil for education funded by loans and medical purposes).
4. The earlier general TCS on sale of goods above ₹50 lakh was withdrawn from April 2025 (TDS on purchase of goods by large buyers continues).
5. Collect at the time of receipt or debit to the buyer, deposit by the 7th of the following month, file quarterly TCS statements and issue certificates.
6. The seller needs a **TAN**; buyers without PAN face higher rates.

## 2. TCS in TallyPrime

1. **F11 → Enable Tax Collected at Source (TCS)** with TAN and collector details.
2. Create a **TCS payable** ledger under Duties & Taxes (Type: TCS) with the nature of goods.
3. Set TCS applicability in the buyer's ledger (PAN, collectee type) and in the sales ledger or stock item (nature of goods).
4. Example: sale of scrap ₹2,00,000 + GST 18% (₹36,000) = ₹2,36,000; TCS 1% on the sale value as per current rules → TallyPrime adds the TCS line to the invoice and the buyer pays the invoice plus TCS.
5. Deposit with **Stat Payment**; generate TCS reports and return data from **Alt+G → TCS Reports**.

## 3. GST TCS for e-commerce

1. E-commerce operators (Amazon, Flipkart, Meesho and others) collect **GST TCS of 0.5%** (0.25% CGST + 0.25% SGST, or 0.5% IGST) on net taxable supplies made through their platforms by sellers, under section 52 of the CGST Act.
2. Operators report it monthly in **GSTR-8**; the amount appears in the seller's **electronic cash ledger** after the seller accepts it, and can be used to pay GST.
3. In TallyPrime, record marketplace settlements: sales at gross value, marketplace commission (with GST, as an expense with ITC), GST TCS (as a receivable/asset ledger until claimed) and income-tax TDS deducted by the operator under the e-commerce provisions (0.1%), then the net bank receipt.

## 4. Reconcile marketplace payments

1. Download settlement reports from the seller portal.
2. Match orders, returns, commissions, shipping fees, TCS and TDS to your books.
3. Reconcile GST TCS with GSTR-2B/TCS credit and accept it on the portal.
4. Claim income-tax TDS through your tax credit statement (Form 26AS/AIS).

## Cheat sheet

| Withholding | Who collects | Rate (examples) | Report |
|---|---|---|---|
| Income-tax TCS | Seller | Scrap 1%, motor vehicle > ₹10 lakh 1% | Quarterly TCS statement |
| LRS TCS | Bank/forex dealer | 20% above ₹10 lakh (certain purposes) | — |
| GST TCS | E-commerce operator | 0.5% | GSTR-8 |
| E-commerce TDS (income tax) | Operator | 0.1% | Operator's TDS return |

## How It Actually Works

TCS places the collection obligation on the party best placed to identify the transaction — sellers of specified goods, banks handling remittances, marketplaces handling sales — creating a trail that ties transactions to taxpayers' PANs and GSTINs. Collected amounts become credits for the payer or seller in their own tax accounts, so recording them as receivable assets (not expenses) and reconciling them with government statements ensures the business actually uses those credits.

## Exercise

Record a scrap sale with GST and income-tax TCS for a buyer with PAN and for one without PAN. Then record a monthly Flipkart settlement for a seller: gross sales ₹3,00,000 including GST, returns ₹20,000, commission ₹36,000 + GST, shipping fees ₹12,000 + GST, GST TCS and TDS, and the net bank receipt. Show the journal and the reconciliation.
