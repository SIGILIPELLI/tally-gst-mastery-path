---
description: "Credit Notes, Debit Notes & Sales Returns — Invoices sometimes need correction after issue: goods returned, price reduced, discount given after sale, or…"
---

# 05 · Credit Notes, Debit Notes & Sales Returns

Invoices sometimes need correction after issue: goods returned, price reduced, discount given after sale, or additional charges. Under GST you never edit an issued invoice to change its tax value — you issue a **credit note** or **debit note**. This module records them correctly.

## 1. When to use which

1. **Credit note** (issued by the supplier) reduces the taxable value or tax of an earlier invoice: sales return, post-sale discount agreed in advance and linked to invoices, price reduction, invoice overcharged.
2. **Debit note** (issued by the supplier) increases value: undercharged price, additional charges.
3. A buyer may issue a "debit note" to a supplier for purchase returns in commercial practice, but under GST the tax adjustment is driven by the **supplier's credit note**.
4. Time limit for GST credit notes: by **30 November** following the end of the financial year (or the annual return date, if earlier).

## 2. Sales return / credit note in TallyPrime

1. Enable **F11 → Use Debit/Credit Notes** (and inventory tracking if items are returned).
2. Press **Ctrl+F8 (Credit Note)**.
3. Party: Srinivasa Stores; select **original invoice number and date** (Reference details — required for GST reporting).
4. Item: Steel Kadai 5 pcs @ ₹600 = ₹3,000; Output CGST ₹270 and SGST ₹270 reversed. Total ₹3,540.
5. Narration: "Return of 5 damaged kadais against Inv. GWM/045".
6. Stock increases by 5 (or post to a damaged-stock item via a stock journal).

## 3. Price reduction without return

1. Use the credit note in **accounting invoice mode** with the sales ledger and tax ledgers, or item mode with zero quantity and value only (configure via F12).
2. Example: agreed 5% discount on Inv. GWM/051 (₹40,000 + IGST ₹7,200): credit note ₹2,000 + IGST ₹360.
3. Discounts not linked to specific invoices or not agreed before supply don't reduce GST value — record them as commercial credit notes without GST.

## 4. Debit note and purchase returns

1. **Ctrl+F9 (Debit Note)** for: (a) your own debit note to a customer for additional charges with GST; or (b) recording a purchase return to a supplier — reference the supplier's original invoice and reverse input tax.
2. Purchase return example: returned 10 LED bulbs @ ₹70 = ₹700 to an inter-state supplier → Input IGST ₹126 reversed. Your ITC drops when the supplier's credit note appears in GSTR-2B.

## 5. Reporting

1. Credit/debit notes to registered parties appear in GSTR-1 **CDNR**; to unregistered parties above thresholds in **CDNUR**; and they adjust GSTR-3B tables.
2. Supplier credit notes reduce your ITC in GSTR-2B.

## Cheat sheet

| Situation | Voucher | Key |
|---|---|---|
| Sales return | Credit Note | Ctrl+F8 |
| Post-sale discount (pre-agreed, linked) | Credit Note | Ctrl+F8 |
| Undercharged / extra charges | Debit Note | Ctrl+F9 |
| Purchase return (record) | Debit Note | Ctrl+F9 |
| Always reference | Original invoice no. & date | |
| Time limit | 30 Nov of next FY | |

## How It Actually Works

GST is reported invoice by invoice, so corrections must also be traceable documents linked to the original supply. A credit note reduces the supplier's output tax and, through GSTR-1 and GSTR-2B, simultaneously reduces the buyer's eligible ITC — keeping both sides of the credit chain consistent. Editing an already-reported invoice would break that link, which is why returns and price changes are always recorded as separate notes.

## Exercise

Record for Godavari Wholesale Mart: a sales return of 5 kadais, a pre-agreed 5% discount credit note on an inter-state invoice, a debit note for ₹1,000 extra freight charged to a customer with GST, and a purchase return to a supplier. Check how each appears in GSTR-1 and in the party ledgers.
