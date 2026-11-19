---
description: "Data Management: Backup, Restore & Split — Losing accounting data is a disaster — years of records, statutory obligations and audit evidence. This module…"
---

# 04 · Data Management: Backup, Restore & Split

Losing accounting data is a disaster — years of records, statutory obligations and audit evidence. This module covers backups, restores, data repair, splitting financial years and moving data between locations in TallyPrime.

## 1. Where data lives

1. Each company is a numbered folder in TallyPrime's **data path** (see **Alt+Y → Data → Data Path** / Company Data settings).
2. Never edit or copy files while TallyPrime has the company open; use TallyPrime's own backup tools.

## 2. Backup

1. **Alt+Y → Backup** (Data menu): choose source companies and a destination (external drive, network folder or a cloud-synced folder).
2. Schedule backups at least **daily** for active companies; TallyPrime's auto-backup options and third-party schedulers help.
3. Follow the **3-2-1 rule**: 3 copies, on 2 different media, 1 off-site (e.g. encrypted cloud storage).
4. Test restores regularly — a backup you can't restore isn't a backup.
5. Protect backups: encrypt (TallyVault) and restrict access.

## 3. Restore and repair

1. **Alt+Y → Restore**: choose the backup file and destination data path; restore to a different path first if you're unsure, to avoid overwriting current data.
2. If a company shows errors (power cut, disk issue), use **Alt+Y → Repair** for the company (always back up first).
3. TallyPrime may also prompt for data migration when moving from older Tally versions (Tally.ERP 9) — follow the migration tool and verify reports before and after.

## 4. Split company by financial year

1. Over years, data grows large. **Alt+Y → Split** divides a company into two: up to a date (e.g. 31-3-2026) and from the next day, carrying closing balances (ledgers, bills, stock) forward as opening balances.
2. Back up before splitting; verify that closing balances in the old company equal opening balances in the new one.
3. Keep the old company read-only (lock period) for audit and reference.
4. Alternatively, continue in one company with multiple years — TallyPrime handles this, but split when performance or management requires.

## 5. Exchanging data

1. **Export/Import** (Alt+E / Alt+O) masters and vouchers in XML or JSON — useful for branch consolidation, migrations and integrations.
2. **Excel import** of masters/vouchers (supported in recent releases) speeds up bulk entry with mapping templates.
3. **Remote access and sync**: TallyPrime offers remote access (browser/app via Tally.NET) and sync between branches; cloud hosting options let multiple users access centrally.

## Cheat sheet

| Task | Path |
|---|---|
| Data path | Alt+Y → Data path settings |
| Backup | Alt+Y → Backup |
| Restore | Alt+Y → Restore (test path first) |
| Repair | Alt+Y → Repair (after backup) |
| Split year | Alt+Y → Split |
| Export/Import | Alt+E / Alt+O |

## How It Actually Works

TallyPrime stores data in its own database files; its backup tool creates a consistent compressed snapshot while ensuring no half-written transactions are captured, which is why copying folders directly can produce corrupt copies. Splitting creates a new company whose opening balances are generated from the old company's closing position, so the two remain reconcilable. Good data management is invisible when it works — and decisive when hardware fails, ransomware strikes or an auditor asks for records from five years ago.

## Exercise

Back up a practice company to an external location, restore it to a different data path and verify its Balance Sheet matches. Split it at a year-end date and confirm closing and opening balances agree. Write a backup policy for a small business (frequency, locations, encryption, test schedule, responsibility).
