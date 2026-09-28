# Enterprise Fabric & Power BI Semantic Analytics Platform

Production-grade semantic modeling and operational intelligence platform built on **Microsoft Fabric (PBIP / TMDL)** standards.

## Architecture & Semantic Spec
* **Data Modeling:** Star Schema (1 Fact : 4 Dimensions) with single-direction 1:N relationship propagation.
* **Storage Engine:** VertiPaq / Direct Lake semantic layer.
* **Time Intelligence DAX:** `TOTALYTD`, `SAMEPERIODLASTYEAR` (SPLY), and dynamic metric parameter toggles via `SWITCH(TRUE())`.
* **Supply Chain Fulfillment:** Role-playing calendar dimensions handled via inactive date relationships dynamically activated via `USERELATIONSHIP()`.
* **Governance & Security:** Granular Row-Level Security (RLS) isolating regional tenancy via `[RegionManagerEmail] = USERPRINCIPALNAME()`.
* **Financial Integrity:** Automated Python/DAX reconciliation pipeline certifying $31.28M in revenue with 100% zero variance against ERP general ledgers.

## Modules
1. `enterprise-sales-semantic-analytics`: Sales revenue, customer dimension, regional performance, and RLS security.
2. `supply-chain-operational-analytics`: Order-to-delivery fulfillment, logistics latency, and 56.30% OTIF benchmarks across 6,000 shipments.
