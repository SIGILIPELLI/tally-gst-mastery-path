---
description: "Foreign Currency & Exports — Businesses that export, import or have foreign customers deal with multiple currencies and exchange rate changes. TallyPrime…"
---

# 07 · Foreign Currency & Exports

Businesses that export, import or have foreign customers deal with multiple currencies and exchange rate changes. TallyPrime handles foreign currency transactions and forex gains/losses, while GST treats exports as **zero-rated**. This module covers both.

## 1. Enable multiple currencies

1. **F11 → Allow Multi-Currency: Yes**.
2. Create currencies: USD ($), EUR (€), AED (د.إ) with symbols and decimal places.
3. Set **Rates of Exchange** (Alt+G → Rates of Exchange) — standard rate, selling and buying rates for dates.
4. In foreign party ledgers (e.g. "Global Home Goods LLC, USA"), set currency USD and registration type **Overseas**.

## 2. Export invoice

1. Sale to a US customer: 500 ceiling fans @ $28 = $14,000, exchange rate ₹84.50 → ₹11,83,000.
2. In the sales invoice, select the foreign ledger; enter rates in USD; TallyPrime converts using the rate.
3. Add export details: port code, shipping bill number and date (for GST reporting).
4. GST treatment (zero-rated supply):
   - **Under LUT** (Letter of Undertaking filed annually on the GST portal): export without paying IGST, then claim refund of unutilised ITC; or
   - **With payment of IGST**, then claim refund of IGST paid (automatically processed via shipping bill data for goods).
5. Exports of services must meet conditions (recipient outside India, payment in convertible foreign exchange or permitted INR, etc.).

## 3. Receipts and forex gain/loss

1. Customer pays $14,000 when the rate is ₹85.10 → bank receives ₹11,91,400.
2. Record the receipt in USD against the invoice; TallyPrime computes the **exchange gain** of ₹8,400 (14,000 × 0.60).
3. Book it with a **forex gain/loss adjustment** (Journal: Dr Customer / Cr Forex Gain, under Indirect Incomes), or let TallyPrime's forex adjustment feature post it.
4. At year-end, **restate** open foreign currency balances at the closing rate and book unrealised gain/loss (the Forex Gain/Loss report helps).

## 4. Imports

1. Purchase from a Chinese supplier in USD; record import duty (customs) and **IGST on imports** paid at customs per the **Bill of Entry**.
2. IGST on imports is claimable as ITC (it appears in GSTR-2B from customs data).
3. Customs duty becomes part of the inventory cost.
4. Import of services: pay IGST under reverse charge (Module 7 of Level 2).

## 5. Compliance reminders

1. Export proceeds must be realised within RBI's prescribed period (currently up to 15 months for goods exports, subject to updates); banks report realisation through the EDPMS system.
2. Keep shipping bills, bills of entry, bank realisation certificates (e-BRC) and LUT copies.
3. GSTR-1 reports exports in **Table 6A**; refunds are claimed on the portal.

## Cheat sheet

| Item | Treatment |
|---|---|
| Currency setup | F11 multi-currency, rates of exchange |
| Export under LUT | No IGST; refund ITC |
| Export with IGST | Pay IGST; refund |
| Forex gain/loss | Realised on receipt; restate at year-end |
| Import IGST | Paid at customs; claim ITC |
| Customs duty | Added to inventory cost |

## How It Actually Works

Foreign currency transactions are recorded at the exchange rate on the transaction date, but settled later at a different rate; the difference is a real gain or loss that must be recognised. TallyPrime tracks the original foreign amount alongside rupee values, so it can compute gains on settlement and restate open balances at the year-end rate. GST zero-rates exports so that Indian goods and services compete internationally without carrying domestic tax, with refunds ensuring input taxes don't become a cost.

## Exercise

Enable multi-currency for Krishna Electricals. Record an export invoice under LUT for $14,000, the receipt at a different rate with the forex gain, an import purchase in USD with customs duty and import IGST, and a year-end restatement of an open USD receivable. Show the GST reporting table for the export.
