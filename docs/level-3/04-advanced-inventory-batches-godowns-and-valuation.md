---
description: "Advanced Inventory: Batches, Godowns & Valuation — As stock grows, you need to know where items are, which batch they came from (for expiry or quality),…"
---

# 04 · Advanced Inventory: Batches, Godowns & Valuation

As stock grows, you need to know **where** items are, **which batch** they came from (for expiry or quality), and **how** stock is valued. This module covers godowns, batches, valuation methods and stock controls in TallyPrime.

## 1. Godowns (locations)

1. **F11 → Maintain Multiple Godowns: Yes**.
2. Create godowns: Main Warehouse, Retail Counter, Nashik Depot, Damaged Stock (with "Our stock with third party" or "Third party stock with us" options for consignment and job work).
3. Every item-based voucher asks for the godown; opening stock can be split by godown.
4. Transfer stock with a **Stock Journal (Alt+F7)** → **Transfer** (e.g. 100 fans from Main Warehouse to Nashik Depot) or use a **Material In/Out** voucher for job work.
5. **Godown Summary** report shows stock by location.

## 2. Batches, expiry and serial numbers

1. **F11 → Enable Batches** (and **Expiry Dates** for medicines, food, chemicals).
2. In the stock item, set **Maintain in batches: Yes**, track date of manufacture and use expiry dates.
3. Enter batch number, manufacturing and expiry dates on purchase; select batches on sale (FEFO — first expiry, first out — for perishables).
4. **Batch-wise reports** and **ageing analysis** reveal slow-moving or near-expiry stock.

## 3. Valuation methods

1. Set per stock item under **Costing method**: **Average Cost** (default), **FIFO**, **Last Purchase Cost**, **Standard Cost**, etc.; and **Market valuation** method for reports.
2. Example — copper wire coils:
   - Opening 100 @ ₹1,800; purchase 200 @ ₹1,950; sold 220.
   - **FIFO**: 100 @ 1,800 + 120 @ 1,950 = ₹4,14,000 COGS; closing 80 @ 1,950 = ₹1,56,000.
   - **Weighted average**: (1,80,000 + 3,90,000) ÷ 300 = ₹1,900; COGS 220 × 1,900 = ₹4,18,000; closing 80 × 1,900 = ₹1,52,000.
3. Accounting standards require inventory at the **lower of cost and net realisable value**; choose a method consistently and disclose it.

## 4. Stock controls

1. **Reorder levels** and minimum order quantities per item/godown → **Reorder Status** report suggests purchases.
2. **Negative stock warnings** (F12) prevent selling stock you don't have.
3. **Physical Stock voucher** (Ctrl+F7) after counts; investigate differences before adjusting.
4. **Price levels** (F11 → Multiple price levels) for wholesale, retail and dealer prices.
5. **Additional cost of purchase** (freight, insurance) can be loaded into item cost for accurate valuation.

## Cheat sheet

| Feature | Use |
|---|---|
| Godowns | Stock by location, transfers |
| Batches & expiry | Traceability, FEFO |
| Costing method | Average, FIFO, last purchase |
| Reorder levels | Automated purchase suggestions |
| Negative stock warning | Prevent overselling |
| Price levels | Different selling prices |

## How It Actually Works

Each item movement records quantity, godown, batch and value. TallyPrime computes cost of goods sold and closing stock by replaying movements under the item's costing method — FIFO consumes the oldest cost layers first, while average cost blends them. Because closing stock directly affects profit, the method you choose changes reported profit when prices rise or fall, which is why consistency and documentation are required by accounting standards and auditors.

## Exercise

Enable godowns and batches for Krishna Electricals. Create three godowns, record purchases in batches across godowns, transfer stock between them, and sell using batch selection. Compute COGS and closing stock for the copper wire example under FIFO and average cost, set it in TallyPrime, and compare the Stock Summary under both methods.
