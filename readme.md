# NYC Yellow Taxi Big Data Analytics on Azure

## Assignment: LDS7005 – Big Data in the Cloud

**Student Name:**  250322385
**Module Leader:** Dr Gayathri Karthick  
**Submission Date:** 28 May 2026  

## Repository Contents

| File | Description |
|------|-------------|
| `New Notebook 2026-05-25 09_53_08.ipynb` | Azure Databricks notebook containing data extraction, cleaning, feature engineering, analytical queries, and linear regression model for fare prediction. |
| `azure_outputs.docx` | Final report with 33 screenshots, architecture diagram, cost analysis table, security configurations, and monitoring evidence. |

## Dataset

- **Source:** NYC Yellow Taxi Trip Data (March 2016) – [Kaggle](https://www.kaggle.com/datasets/elemento/nyc-yellow-taxi-trip-data?select=yellow_tripdata_2016-03.csv)
- **Size:** ~1.9 GB (19 columns, ~12 million records after cleaning)

## Azure Services Used

- Azure Data Lake Storage Gen2 (ADLS Gen2)
- Azure Databricks (auto‑scaling cluster, min 1, max 8 workers)
- Azure Synapse Analytics (dedicated SQL pool, external tables on Delta Lake)
- Azure Monitor & Log Analytics
- Azure Key Vault (for secrets – described in report)
- Azure Cost Management

## Key Results

- **Peak hour:** 7 PM (754,522 trips) – 17% higher average fare
- **Tip analysis:** Weekdays average 10.6%, weekends 9.8%
- **ML model:** Linear regression – R² = 0.9466, RMSE = 2.40
- **Cost optimisation:** Optimised monthly cost £4.58 vs. non‑optimised £441.42

## How to Run the Notebook (For Marker)

1. Import the `.ipynb` file into an Azure Databricks workspace.
2. Attach to a cluster (standard, not serverless) with Spark 4.0+.
3. Replace the storage account key and container names with your own.
4. Run all cells sequentially.

## References

All academic and official references are listed in the report (`draf-1.docx`).

---

**Note:** The dataset is not stored in this repository due to size limits. Use the Kaggle link above to download it.
