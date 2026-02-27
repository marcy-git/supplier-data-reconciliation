# 📦 Supplier Data Reconciliation

## 🔍 Overview
Automated reconciliation process to identify discrepancies between 
supplier backlog and internal Purchase Orders using Power Query in Excel.

## 🛠️ Tools
- Microsoft Excel
- Power Query

## 📊 Dataset
- 314 Purchase Orders
- 37 unique Part Numbers
- Fields: PO, PN, Quantity, CRD, ETA, Unit Price

## 💡 Business Problem
Manual cross-checking of 300+ POs was time-consuming and error-prone.
Discrepancies in quantities or dates can cause inventory and billing issues.

## ✅ Solution
Built a Power Query model that merges both data sources and flags 
field-level mismatches with a clear action column (YES, UPDATE).

## 📈 Impact
- Reduced reconciliation time from hours to minutes
- Repeatable process reusable every planning cycle
