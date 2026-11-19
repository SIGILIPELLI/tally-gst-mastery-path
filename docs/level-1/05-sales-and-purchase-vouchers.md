---
description: "Sales & Purchase Vouchers — Buying and selling goods are the heart of a trading business. This module records purchases and sales in TallyPrime — first in…"
---

# 05 · Sales & Purchase Vouchers

Buying and selling goods are the heart of a trading business. This module records purchases and sales in TallyPrime — first in **accounting invoice** mode (amounts only), then **item invoice** mode with inventory (after Module 6, you'll use items routinely).

## 1. Purchase voucher (F9)

1. Bought goods on credit from Lakshmi Paper Mart, Bill No. LPM/221, ₹80,000.
2. Open **F9 Purchase**. Set **Supplier invoice no.** and date (important for GST and payments later).
3. **Party A/c name**: Lakshmi Paper Mart; **Purchase ledger**: Purchases.
4. In accounting invoice mode, enter the amount ₹80,000. Add freight ₹1,500 as an additional ledger line (Freight Inward, Direct Expenses) if it's on the same bill.
5. Narration: "Purchase of notebooks and pens, bill LPM/221". Save with **Ctrl+A**.
6. For **cash purchases**, select Cash as the party ledger.

## 2. Sales voucher (F8)

1. Sold goods on credit to Vijay Book Stall, ₹50,000.
2. Open **F8 Sales**. TallyPrime numbers sales invoices automatically.
3. **Party A/c name**: Vijay Book Stall; **Sales ledger**: Sales.
4. Enter the amount; add any extra charges (e.g. packing charges collected, under Indirect Incomes) as separate lines.
5. Print the invoice with **Alt+P** (configure logo, bank details and terms under print configuration).
6. For **cash sales**, choose Cash as the party.

## 3. Item invoice mode (with inventory)

1. With **Maintain Inventory** on, press **Ctrl+H (Change Mode)** in the voucher and choose **Item Invoice**.
2. Select the **stock item**, enter quantity and rate; TallyPrime calculates the amount and updates stock.
3. Example sale: 200 Classmate notebooks @ ₹45 = ₹9,000; 100 Reynolds pens (boxes of 10) @ ₹60 = ₹6,000; total ₹15,000.
4. Add discounts per line (enable via F12) or as a separate Discount Allowed ledger.

## 4. Orders, delivery and receipt notes (overview)

1. Larger businesses track the cycle: **Purchase Order → Receipt Note (goods received) → Purchase invoice**, and **Sales Order → Delivery Note → Sales invoice**.
2. Enable via **F11 → Enable Order Processing**. Delivery Note (**Alt+F8**) and Receipt Note (**Alt+F9**) record goods movement before billing.
3. Outstanding orders reports show what's pending — useful for wholesalers like Sri Sai Traders.

## Cheat sheet

| Task | Path / key |
|---|---|
| Purchase | F9 |
| Sales | F8 |
| Accounting vs item invoice | Ctrl+H (Change Mode) |
| Supplier invoice no. | Enter on every purchase |
| Print invoice | Alt+P |
| Delivery / Receipt Note | Alt+F8 / Alt+F9 |
| Order processing | F11 |

## How It Actually Works

A sales voucher posts a debit to the customer (or cash) and a credit to the sales ledger; with inventory, it also reduces stock quantity and records the outward movement at the item's cost for valuation. Purchase vouchers do the reverse. Because the party, invoice number, date and items are captured in one record, TallyPrime can later produce GST returns, outstanding reports and stock statements from the same data — which is why accurate invoice details matter far beyond the entry itself.

## Exercise

Record: purchase from Lakshmi Paper Mart ₹80,000 + freight ₹1,500 (bill LPM/221); cash purchase ₹6,000; credit sale to Vijay Book Stall ₹50,000; cash sale ₹22,000; credit sale to another customer ₹18,500. Print one sales invoice. Check the Sales and Purchase registers (Alt+G → Sales Register / Purchase Register).
