---
description: "E-Invoicing & E-Way Bills — Two electronic systems sit alongside GST invoices: e-invoicing, which registers B2B invoices with a government portal, and…"
---

# 06 · E-Invoicing & E-Way Bills

Two electronic systems sit alongside GST invoices: **e-invoicing**, which registers B2B invoices with a government portal, and **e-way bills**, which document goods in transit. TallyPrime can generate both directly. Thresholds are as of 2026 — confirm on einvoice.gst.gov.in and ewaybillgst.gov.in.

## 1. E-invoicing basics

1. Mandatory for taxpayers whose **aggregate annual turnover exceeds ₹5 crore** in any financial year since 2017-18 (certain sectors like banks, insurers, SEZ units and GTAs are exempt).
2. Applies to B2B invoices, exports, and credit/debit notes to registered persons — not B2C invoices (those may need a dynamic QR code above a higher turnover threshold).
3. The invoice is reported to the **Invoice Registration Portal (IRP)**, which validates it and returns an **IRN** (Invoice Reference Number), an acknowledgement number and date, and a **signed QR code** that must be printed on the invoice.
4. Taxpayers with turnover of **₹10 crore and above** must report invoices to the IRP within **30 days** of the invoice date.
5. E-invoice data flows automatically into the supplier's GSTR-1 and can auto-generate an e-way bill.

## 2. E-invoicing in TallyPrime

1. In company GST details, set **e-Invoicing applicable: Yes** and the applicable date.
2. Ensure masters are complete: party GSTIN, address, pincode, state; item HSN; unit mapped to UQC.
3. On saving a sales invoice, TallyPrime offers to **Send for e-Invoicing** (connected services require a Tally.NET/IRP login setup with your GSP credentials).
4. TallyPrime stores the IRN, acknowledgement and QR code and prints them on the invoice.
5. Cancel an IRN within **24 hours** if needed (cancel on IRP, then in TallyPrime); after that, issue a credit note.
6. The **e-Invoice report** lists invoices pending, sent, rejected or cancelled.

## 3. E-way bill basics

1. Required for movement of goods where the consignment value exceeds **₹50,000** (some states have different limits for intra-state movement), with exemptions for certain goods.
2. **Part A**: GSTINs of supplier and recipient, place of delivery, invoice number/date, value, HSN, reason for transport.
3. **Part B**: transporter details — vehicle number (road) or transport document number (rail, air, ship).
4. Validity depends on distance: generally **1 day per 200 km** for regular cargo (20 km per day for over-dimensional cargo).
5. The person causing movement (usually the supplier, or the transporter/recipient) generates it.

## 4. E-way bills in TallyPrime

1. Enable e-Way Bill in GST details with the threshold limit and applicable date.
2. In the sales invoice, fill **e-Way Bill details**: transporter, distance (pincode-based), mode, vehicle number.
3. Generate online through TallyPrime's connected services or export JSON for upload on the e-way bill portal.
4. Update Part B if the vehicle changes; extend validity before expiry if transit is delayed.
5. The **e-Way Bill report** shows bills pending generation, generated and expiring.

## Cheat sheet

| Item | Rule (2026) |
|---|---|
| E-invoice threshold | AATO > ₹5 crore |
| Output | IRN + signed QR on invoice |
| 30-day reporting | AATO ≥ ₹10 crore |
| IRN cancellation | Within 24 hours |
| E-way bill threshold | Consignment > ₹50,000 (state variations) |
| E-way validity | ~1 day per 200 km |

## How It Actually Works

E-invoicing moves invoice reporting to the moment of issue: the IRP validates the invoice's structure and the supplier's identity, stamps it with a unique IRN and passes the data to the GST and e-way bill systems. This reduces fake invoices and data mismatches because buyers' credit is based on validated records. E-way bills track goods physically moving, letting tax officers verify consignments on the road against declared invoices; the e-invoice-to-e-way-bill link means one accurate entry serves both.

## Exercise

For Godavari Wholesale Mart (assume turnover above ₹5 crore), configure e-invoicing and e-way bills, complete all required master fields, and prepare one B2B invoice with e-invoice and e-way bill details (vehicle, distance 275 km). State the e-way bill validity and the latest time the IRN could be cancelled.
