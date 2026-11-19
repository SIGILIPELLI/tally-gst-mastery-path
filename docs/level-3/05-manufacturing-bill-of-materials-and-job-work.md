---
description: "Manufacturing: Bill of Materials & Job Work — Manufacturers turn raw materials into finished goods. TallyPrime records this with a Bill of Materials (BOM)…"
---

# 05 · Manufacturing: Bill of Materials & Job Work

Manufacturers turn raw materials into finished goods. TallyPrime records this with a **Bill of Materials (BOM)** and **manufacturing journals**, and handles **job work** — sending materials to others for processing, or processing for others. Our example: *Deccan Furniture Works* makes study tables.

## 1. Set up a Bill of Materials

1. In the finished stock item "Study Table – Standard", set **Set components (BoM): Yes**.
2. Define components per 1 unit: Plywood sheet 1 No, Teak legs 4 Nos, Screws 32 Nos, Laminate 1.5 sq m, Drawer runners 1 set; optional scrap/by-product: wood waste 0.5 kg.
3. Specify **godowns** for components and output, and multiple BOMs if there are variants.
4. Raw materials are separate stock items with their own costs and GST details.

## 2. Record production

1. Use **Stock Journal (Alt+F7) → Manufacture** (or a Manufacturing Journal voucher type).
2. Select the finished item and quantity (e.g. 20 tables); TallyPrime fills components from the BOM (20 plywood sheets, 80 legs, 640 screws, 30 sq m laminate, 20 runner sets).
3. Add **additional costs** of manufacturing — direct labour ₹12,000, power ₹3,000 — so the finished goods cost includes them.
4. Finished goods cost per table = (components + additional costs) ÷ 20.
5. Stock of raw materials decreases and finished goods increases; accounts reflect values through stock valuation.

## 3. Job work — sending materials out (principal)

1. **F11 → Enable Job Order Processing**.
2. Create a **Job Work Out Order** to the job worker (e.g. polishing unit), then **Material Out** voucher to send tables for polishing.
3. Record **Material In** when polished goods return, and the job worker's purchase invoice for processing charges (with GST).
4. Under GST, goods sent for job work move on a **delivery challan** without tax; inputs must return within **1 year** and capital goods within **3 years**, or they're treated as supplies.
5. Report job work movements in the **ITC-04** form (annual or half-yearly depending on turnover, as currently applicable).

## 4. Job work — processing for others (job worker)

1. Create a **Job Work In Order** from the principal.
2. **Material In** records the principal's goods received (tracked as third-party stock, not yours).
3. Record consumption and **Material Out** when returning processed goods.
4. Raise a sales invoice for **job work charges** (services, with applicable GST rate and SAC).

## Cheat sheet

| Task | Voucher |
|---|---|
| Define recipe | BoM in stock item |
| Production | Stock Journal → Manufacture |
| Add labour/overheads | Additional cost in manufacture |
| Send to job worker | Job Work Out Order → Material Out |
| Receive back | Material In + job worker invoice |
| Process for others | Job Work In Order → Material In/Out |
| GST report | ITC-04 |

## How It Actually Works

A BOM is a recipe that tells TallyPrime how much of each input one unit of output consumes, so a single manufacture entry moves dozens of stock quantities consistently. The finished item's cost is built from component costs plus loaded overheads, which feeds inventory valuation and gross margin. Job work tracking keeps ownership clear — materials at a job worker remain the principal's stock — which matters for valuation, insurance and the GST rules that allow tax-free movement only within time limits.

## Exercise

Create raw materials and a BOM for a study table, record opening raw material stock, manufacture 20 tables with labour and power costs, and compute the cost per table. Then send 10 tables to a polishing job worker, receive them back, and record the job worker's invoice with GST.
