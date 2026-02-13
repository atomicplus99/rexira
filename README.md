# REXIRA

Retail ERP designed around real-world events instead of mutable state.

Most POS systems store current values (stock, balance) but cannot reconstruct what actually happened.  
REXIRA models business operations as auditable transactions.

---

## Key Ideas

- A product is not inventory
- A sale is not money
- Stock is never edited directly
- History is immutable
- Profit is calculated from real cost batches

---

## System Goals

- Inventory traceability by batch
- Financial consistency
- Reproducible historical reports
- Separation of commercial and monetary flows

---

## Project Status

This repository currently contains the domain specification and architectural decisions before implementation.

The objective is to design the system correctly before choosing technologies.

---

## Why this project

The goal of REXIRA is to demonstrate backend engineering skills through real-world business modeling rather than CRUD application development.
