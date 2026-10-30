# Drug Price-Regulation System (showcase)

> The source code belongs to the client and stays private. This repository describes what was built.

A system for a national drug authority that runs the full medicine pricing chain, from a company's appeal to the final approved price, plus import and release approvals and warehouse stock.

**Status:** live at the client, with regular update packages.

## The problem
Prices were decided through a chain of paper documents: company appeals, price studies, committee minutes and final approvals. Nothing linked them, invoices came in dollars, riyals and euros, and the old database couldn't be shared.

## What I built
- **Linked document chain:** appeal → price study → change request → decision minutes → final approval. Each step creates the next.
- **No silent edits:** approved documents are corrected by numbered revisions, never edited.
- **Multi-currency:** each document stores the original amount and freezes the exchange rate used.
- **Security:** 95 permissions across 8 roles, separation of duties, JWT, CSP headers, full audit trail of before/after values.
- **Operations:** one-click Windows installer, scheduled backups, restore script, update packages.
- **Data import:** items imported from Excel and CSV with duplicate detection.

## Quality
- ~300 automated unit and integration tests
- SRS, SDD, ERD, 38 sequence diagrams and an Arabic user manual

## Stack
.NET 8 · ASP.NET Core · EF Core · SQL Server · React 19 · TypeScript · Ant Design (RTL) · TanStack Query

---
Built by **Bashar Ahmed Abdullah** · [BashX](https://YOUR-DOMAIN) · [Case study](https://YOUR-DOMAIN/#case-studies)
