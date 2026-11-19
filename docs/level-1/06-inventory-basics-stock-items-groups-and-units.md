---
description: "Inventory Basics: Stock Items, Groups & Units — For a trading business, stock is usually the largest asset. TallyPrime's inventory module tracks…"
---

# 06 · Inventory Basics: Stock Items, Groups & Units

For a trading business, stock is usually the largest asset. TallyPrime's inventory module tracks quantities, values and movement of every item. This module sets up units, stock groups and items, and records stock-based vouchers.

## 1. Units of measure

1. **Alt+G → Create Master → Unit**.
2. **Simple units**: Nos (numbers), Box, Kg, Pcs, Ream. Set the symbol and decimal places (0 for Nos).
3. **Compound units**: Box of 10 Nos — lets you sell in boxes and track pieces.
4. For GST later, map each unit to the official **UQC** (Unit Quantity Code), e.g. Nos → NOS-NUMBERS.

## 2. Stock groups and categories

1. **Stock groups** organise items: Notebooks, Pens, Paper, Art Supplies.
2. **Stock categories** (optional, F11/F12) add a second classification such as brand: Classmate, Reynolds, JK Paper.
3. Create via **Alt+G → Create Master → Stock Group / Stock Category**.

## 3. Stock items

1. **Alt+G → Create Master → Stock Item**.
2. Fill name ("Classmate Notebook 172 pages"), group (Notebooks), category, unit (Nos).
3. **Opening balance**: quantity 500, rate ₹38 → value ₹19,000.
4. Later you'll add GST details (HSN code and rate) on items.
5. Set **standard rates** (cost/selling price) if your business uses fixed price lists.

Example items for Sri Sai Traders:

| Item | Group | Unit | Opening qty | Rate |
|---|---|---|---|---|
| Classmate Notebook 172 pages | Notebooks | Nos | 500 | 38 |
| Reynolds Pen Box (10) | Pens | Box | 200 | 52 |
| JK Copier A4 Ream | Paper | Ream | 150 | 230 |

## 4. Recording stock movement

1. Purchases (**F9**) and sales (**F8**) in item invoice mode update quantities automatically.
2. **Stock Journal (Alt+F7)** transfers or converts stock — e.g. damaged items moved to a "Damaged" item, or repacking.
3. **Physical Stock voucher (Ctrl+F7)** records actual counted quantities; TallyPrime adjusts book stock to match.
4. Enable **godowns/locations** later (Level 3) if stock is kept in more than one place.

## 5. Inventory reports

1. **Stock Summary** (Alt+G → Stock Summary): quantity, rate and value of every item.
2. **Stock Item vouchers**: movement history for one item.
3. **Movement Analysis**: which items sell fastest.
4. **Reorder status** (after setting reorder levels): items to buy.
5. Valuation method defaults to **Average Cost**; others (FIFO, Last Purchase Cost) are set per item (Level 3).

## Cheat sheet

| Master / voucher | Path or key |
|---|---|
| Unit | Create Master → Unit |
| Stock Group / Category | Create Master → Stock Group / Category |
| Stock Item | Create Master → Stock Item |
| Stock Journal | Alt+F7 |
| Physical Stock | Ctrl+F7 |
| Stock Summary | Alt+G → Stock Summary |

## How It Actually Works

When inventory is integrated with accounts, every item-based voucher updates both quantity and value. Closing stock is calculated automatically using the item's valuation method and flows into the Balance Sheet (as an asset) and the P&L (reducing cost of goods sold). That integration means stock errors become profit errors — an unrecorded sale overstates stock and understates profit, which is why periodic physical counts and the Physical Stock voucher matter.

## Exercise

Create the three units, four stock groups and the three items above with opening stock. Record an item-wise purchase of 300 Classmate notebooks @ ₹39, an item-wise sale of 250 notebooks @ ₹48 and 50 pen boxes @ ₹65, and a physical stock count showing 498 reams of A4 instead of the book quantity. Review the Stock Summary.
