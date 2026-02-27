# 📦 Supplier Data Reconciliation — Supply Chain Analytics

## Project Overview

Developed an automated data reconciliation process to identify discrepancies between the supplier's backlog and internal Open Purchase Orders (POs), enabling the procurement team to take timely corrective actions and maintain data accuracy across systems.

## Business Problem

In Supply Chain operations, data misalignment between a supplier's records and internal ERP/system data is a common and costly issue. Discrepancies in quantities, delivery dates (CRD/ETA), or pricing can lead to:
- Incorrect inventory planning
- Missed delivery commitments
- Billing disputes with suppliers

Manual cross-checking of 300+ POs was time-consuming and error-prone. A structured, repeatable process was needed.

## Solution

Built a Power Query-based reconciliation model in Excel that:
1. **Ingests two data sources**: Supplier's Backlog export and internal Open PO report
2. **Merges both datasets** on PO number and Part Number (PN) as keys
3. **Compares field by field**: Quantity, CRD (Customer Required Date), ETA, and Unit Price
4. **Flags discrepancies** with MATCH / MISMATCH status per field
5. **Generates an action flag** (`YES, UPDATE`) for any PO requiring follow-up

## Tools & Techniques

| Tool | Usage |
|---|---|
| **Power Query (Excel)** | Data ingestion, merging, transformation |
| **Excel** | Final reconciliation table, conditional formatting |
| **Data Matching Logic** | Field-level comparison across 6 attributes |

## Dataset

- **314 Purchase Orders** across both sources
- **37 unique Part Numbers**
- Fields analyzed: PO, PN, Quantity, CRD, ETA, Unit Price

## Key Outputs

- Reconciliation table with clear MATCH/MISMATCH status per field
- Action column identifying POs that require immediate update
- Color-coded dashboard for quick visual review (green = OK, red = MISMATCH, yellow = action needed)

## Impact

- Reduced manual reconciliation time from hours to minutes
- Provided a repeatable, scalable process reusable every planning cycle
- Improved supplier communication by providing structured discrepancy reports

## Skills Demonstrated

`Power Query` · `Data Reconciliation` · `Supply Chain Analytics` · `Excel` · `Data Quality` · `Procurement Operations`

---

*Note: Data has been anonymized. PO numbers and Part Numbers have been replaced with generic identifiers to protect confidentiality.*
