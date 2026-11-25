# Northstar Finance — Independent Accounts UI

This is a separate Finance & Accounts project, not Pulse ERP.

## Run
```bash
npm install
npm run dev
```

## What is different in this version
The previous version used one generic table template across most routes. This version has separate page-workspace components for the functional areas: dashboard, invoice/bill document editors, account hierarchy, journal composer with debit-credit balance, bank reconciliation, statement import and mapping, cash register, GST overview and return workpapers, TDS/TCS, financial statements, ledgers, trial balance, ageing, partner profile, receipt allocation, payment batch/refund, credit/debit notes, bank accounts, provider catalogue, OCR review, review queue, audit timeline, working files, period close, regularization, fixed assets, depreciation, deferred schedules, loans, fiscal periods/locks, currencies, fiscal positions, tax master/report, reminders, integrations, document templates, permissions and company accounting setup.

Navigation includes Dashboard, Customers, Vendors, Accounting, Banking, Tax & Compliance, Review, Reporting and Configuration. Each destination has a different renderer and layout based on its purpose. Some closely related list destinations use the same list component but have their own columns and feature-specific data; complex workflows have dedicated workspaces.

## Source specification handling
The UI scope is based on `Finance_Module_Feature_Specification.pdf` (15 pages). The specification explicitly says that the detailed behavior of Customer Products, Vendor Products and PAN Entity is not fully evidenced; those pages are provided without inventing unverified business rules.

## Prototype boundary
This is frontend-only with illustrative sample records and simulated interactions. It does not persist records to a backend or execute real postings, statutory tax calculations/filings, bank synchronization, payment provider transactions, OCR extraction, permissions, or immutable audit. Financial calculations and access checks must be authoritative on a secure backend before production use.
