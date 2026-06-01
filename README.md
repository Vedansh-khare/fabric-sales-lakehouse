![Azure Data Factory](https://img.shields.io/badge/Azure%20Data%20Factory-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![ADLS Gen2](https://img.shields.io/badge/ADLS%20Gen2-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Git](https://img.shields.io/badge/Git%20CI%2FCD-F05032?style=for-the-badge&logo=git&logoColor=white)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)
# fabric-sales-lakehouse

# 🏭 Sales Analytics Lakehouse | ADF + Azure Portfolio

> Enterprise ETL migrated from Informatica PowerCenter to Azure Data Factory + ADLS Gen2 Medallion Architecture

## 🏗️ Architecture

CSV Source (AdventureWorks) → [Bronze Layer] Raw Files in ADLS Gen2 → [Silver Layer] Cleaned, typed data → [Gold Layer] Aggregated analytics

## 🛠️ Tech Stack
- Azure Data Factory (V2)
- Azure Data Lake Storage Gen2
- Delta Lake / Parquet
- Python / PySpark
- GitHub Actions CI/CD

## 📊 Dataset
AdventureWorks Sales — Microsoft sample database

## 🔄 Informatica → ADF Migration Map
| Informatica | ADF Equivalent |
|---|---|
| Mapping | Data Flow |
| Session | Pipeline Activity |
| Workflow | Pipeline |
| Source/Target | Linked Service + Dataset |

## Pipeline Run — All Green ✅

![Pipeline Success](docs/pipeline-success.png)

## Architecture

![Architecture](docs/architecture.png)

## 👤 Author
Vedansh Khare | Informatica ETL → Azure Data Engineer
