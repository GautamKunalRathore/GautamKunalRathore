## Gautam Kunal

**I build in-house ERP systems for manufacturing companies, from the factory floor to payroll.**

Business Intelligence Manager at **Eureka Windoor Systems** (EUMAX and WINDIA uPVC profiles; plants in Bengaluru, Ghaziabad and Hyderabad). I own product and technical direction for the company's custom ERP, built module by module and running live in production.

> My production work lives in private company repositories. This page describes what those systems do and how they are built. No proprietary code is shared here.

---

### Systems I've built and run

| System | What it does | Status |
|---|---|---|
| **MEIP** (Manufacturing Execution & Intelligence Platform) | Production tracking per extrusion line, barcoded bundle labels on thermal printers, QC accept/reject, warehouse scan stations, automatic downtime capture, lamination module | Live on the factory floor |
| **HRMS & Payroll** | Monthly payroll for direct staff and vendor/contract workforce, statutory PF, vendor invoicing, deductions, approval reports for management. Expanding to biometric attendance and hiring-to-onboarding | Live; migrating to Next.js |
| **Projects Tracker** | Tracks every doors-and-windows order from booking to site installation. Offline-first, because site connectivity is poor | Live |
| **Production Forecast** | MIN/MAX finished-stock model for 360+ SKUs at a 95% service level, with per-tool run physics and batch cadence | In use for planning |

### Engineering highlights

- Migrated Google Apps Script / Sheets prototypes to **Next.js + Supabase (Postgres) + Vercel**, running old and new systems in parallel until cut-over
- Wrote a **print agent** that generates TSPL and drives thermal label printers through the Windows spooler; made the print queue idempotent (lease-based claim, lease reaper, dedupe ledger) to stop duplicate labels
- **Schema-per-module Postgres design** with audit trails and application-level role permissions
- **Offline-first** web app for installation sites with weak networks
- PR-based workflow with regular dependency and security upgrades across three production apps

### Stack

`Next.js` `React` `TypeScript` `Node.js` `Supabase` `PostgreSQL` `Vercel` `Google Apps Script` `Python` `Excel modelling`

### How I work

- Start from the business process, write the rules down, then build
- Ship to live users without stopping the floor: parallel runs, audit trails, rollback paths
- One owner across the whole loop: requirements, data model, code, deployment, training

### Contact

[Portfolio](https://gautamkunal.netlify.app) · [LinkedIn](https://www.linkedin.com/in/gautamkunalrathore) · gautamkunal0007@gmail.com

Open to roles where a company needs someone to build its core systems end to end.
