# Changelog

All notable changes to this project documented here.

---

## [1.0.0] — 2025-06-01

### Added
- `pl_bronze_ingest` pipeline — 4 chained Copy Activities ingesting AdventureWorks CSVs (Customer, SalesOrderHeader, SalesOrderDetail, Product) into ADLS Gen2 Bronze container
- `df_silver_transform` Data Flow — RenameColumns → FilterNulls → DerivedColumns (ingestion_date, source_system) → Gold sink
- `ds_gold_salesorders` dataset → `gold/sales_orders_gold.csv`
- `tr_daily_6am` schedule trigger — daily at 6AM IST, no end date
- Linked Services: ADLS Gen2 + ADF Git integration
- GitHub CI/CD — ADF auto-commits on publish to `main` branch
- `docs/pipeline-success.png` — full pipeline run screenshot (all 5 activities green)
- `docs/architecture.png` — medallion architecture diagram (Bronze → Silver → Gold)

### Infrastructure
- Resource group: `fabric-portfolio-rg` (Central India)
- Storage: `vedanshstorage001` (ADLS Gen2, hierarchical namespace ON)
- Containers: `bronze`, `silver`, `gold`

---

## [Unreleased]

### Planned
- ADF Repo 2: Complex transforms — multi-table joins, aggregations, window functions
- ADF Repo 3: CI/CD pipeline + error handling + alerting
- Microsoft Fabric Repo 1: Medallion Lakehouse
