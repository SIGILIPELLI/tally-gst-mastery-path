---
description: "GST Invoicing: HSN/SAC, Tax Rates & Place of Supply — A GST invoice must contain specific details, and TallyPrime calculates tax automatically once…"
---

# 02 · GST Invoicing: HSN/SAC, Tax Rates & Place of Supply

A GST invoice must contain specific details, and TallyPrime calculates tax automatically once masters are right. This module records intra-state, inter-state, B2B and B2C sales and purchases correctly.

## 1. Mandatory tax invoice contents

1. Supplier name, address and **GSTIN**.
2. Consecutive serial number unique for the financial year (up to 16 characters) and date.
3. Recipient name, address and GSTIN (for registered buyers); for unregistered buyers above certain values, name, address and state.
4. **HSN/SAC**, description, quantity, unit, value, discount, taxable value.
5. Tax rate and amount separately for CGST, SGST/UTGST, IGST.
6. **Place of supply** (state name) for inter-state supplies.
7. Whether tax is payable on reverse charge, and signature.
8. For unregistered buyers or composition dealers, a **Bill of Supply** is used when no tax is charged (e.g. by composition dealers or for exempt goods).

## 2. Intra-state sale (CGST + SGST)

1. **F8 Sales** → Party: Srinivasa Stores, Vijayawada (registered, Andhra Pradesh).
2. Item: Steel Kadai 20 pcs @ ₹600 = ₹12,000 (18%).
3. Add **Output CGST** and **Output SGST** ledgers below items — TallyPrime fills ₹1,080 each.
4. Invoice total ₹14,160. Print with **Alt+P**; the invoice shows HSN, rates and tax split.

## 3. Inter-state sale (IGST)

1. Party: Sai Ram Traders, Hyderabad (Telangana, registered).
2. Item: LED Bulbs 9W 500 pcs @ ₹70 = ₹35,000 at the item's GST rate.
3. Add **Output IGST** — at 18%, ₹6,300; total ₹41,300.
4. TallyPrime sets **Place of Supply: Telangana** from the party; you can change it in party details if goods are delivered elsewhere (e.g. "bill to" one state, "ship to" another — enter dispatch and consignee details).

## 4. B2C sales and purchases

1. Walk-in customer (unregistered): use a **Cash** or "Retail Customer" ledger with registration type Unregistered/Consumer; tax is calculated the same way.
2. Inter-state B2C invoices above **₹1 lakh** are reported individually in GSTR-1 (B2CL); smaller B2C sales are summarised (B2CS).
3. **F9 Purchase** from a registered supplier: enter supplier invoice number and date exactly as on their bill, items, and **Input CGST/SGST** or **Input IGST**. These must match the supplier's GSTR-1 for your ITC.

## 5. Check invoice-level GST

1. Use **Alt+G → GSTR-1** later to see how each invoice is classified (B2B, B2CL, B2CS, exports).
2. Open any voucher and press **Ctrl+O** (Related Reports) or view **Tax Analysis** (via **Ctrl+I**/More Details in recent releases) to see the tax break-up.
3. If a voucher shows as "uncertain" or "incomplete" in GST reports, it lacks details (GSTIN, HSN, state) — fix the masters or voucher.

## Cheat sheet

| Scenario | Tax | Notes |
|---|---|---|
| Same state, registered buyer | CGST + SGST | B2B in GSTR-1 |
| Different state, registered | IGST | Place of supply = buyer state |
| Unregistered, inter-state > ₹1 lakh | IGST | B2CL |
| Unregistered, other | As applicable | B2CS summary |
| Purchase | Input CGST/SGST or IGST | Match supplier invoice no. |

## How It Actually Works

Each GST invoice becomes a data record that flows to your GSTR-1 and, from there, to your buyer's GSTR-2B as eligible ITC. That chain is why invoice numbers, dates, GSTINs and HSN codes must be exact — a typo on your sale can deny your customer their credit. TallyPrime classifies invoices into GSTR-1 tables automatically based on registration type, place of supply and invoice value, and flags records with missing information before you file.

## Exercise

In Godavari Wholesale Mart, record: an intra-state B2B sale, an inter-state B2B sale to Telangana, an inter-state B2C sale above ₹1 lakh, a cash B2C sale, and two purchases (one intra-state, one inter-state). Print one invoice of each type and verify the tax split. Open GSTR-1 and confirm each sale's table.
