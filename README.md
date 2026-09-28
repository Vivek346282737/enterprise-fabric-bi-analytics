# Enterprise Fabric & Power BI Semantic Analytics Platform

[![Microsoft Fabric](https://img.shields.io/badge/Platform-Microsoft%20Fabric-0078D4?style=for-the-badge&logo=microsoft)](https://www.microsoft.com/en-us/microsoft-fabric)
[![Power BI](https://img.shields.io/badge/BI-Power%20BI%20Desktop%20%2F%20Service-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![Semantic Format](https://img.shields.io/badge/Format-PBIP%20%7C%20TMDL-2374AB?style=for-the-badge)](https://learn.microsoft.com/en-us/power-bi/developer/projects/projects-overview)
[![Engine](https://img.shields.io/badge/Engine-VertiPaq%20%2F%20Direct%20Lake-107C41?style=for-the-badge)](https://learn.microsoft.com/en-us/analysis-services/tabular-models/tabular-models-ssas)
[![RLS Enforced](https://img.shields.io/badge/Security-Row--Level%20Security%20(USERPRINCIPALNAME)-critical?style=for-the-badge)](https://learn.microsoft.com/en-us/power-bi/enterprise/service-admin-rls)
[![Reconciliation](https://img.shields.io/badge/UAT%20Audit-%2431.28M%20Reconciled%20(0%20Variance)-success?style=for-the-badge)](#financial-reconciliation--audit-sign-off)

---

## Executive Summary
This repository houses an enterprise-grade Business Intelligence and Operational Intelligence solution architected natively for **Microsoft Fabric (PBIP / TMDL Developer Mode)**. Departing from legacy monolithic `.pbix` workflows, the platform enforces modern code-first engineering practices: source-controllable Tabular Model Definition Language (`.tmdl`), git-integrated semantic layers, deterministic DAX measure libraries, granular Row-Level Security (RLS), and automated source-to-report reconciliation pipelines.

The platform orchestrates **5,000+ sales transactions** and **6,000+ logistics shipment events**, balancing financial revenue reporting ($31.28M certified ledger) against operational fulfillment efficiency (56.30% OTIF benchmarks).

---

## Architecture & Semantic Topology

The analytical engine runs on an optimized **Star Schema (Kimball Methodology)** designed for sub-second VertiPaq compression and cache efficiency: