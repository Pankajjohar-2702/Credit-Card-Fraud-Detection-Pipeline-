# 💳 Credit Card Fraud Detection Pipeline

An end-to-end **Data Engineering project** demonstrating how credit card transaction data can be ingested, processed, transformed, stored and visualised using Microsoft Azure services, Python, PySpark and Power BI.

The project follows the **Medallion Architecture (Bronze, Silver and Gold)** to organise transaction data into structured processing layers and prepare it for analytical reporting.

---

## 📌 Project Overview

The Credit Card Fraud Detection Pipeline demonstrates a cloud-based data engineering workflow for processing and analysing credit card transactions.

The pipeline integrates multiple technologies to create a structured data processing environment, starting from source data preparation and ending with interactive dashboard visualisation.

The main objective is to understand how modern cloud data engineering tools work together to manage, transform and analyse large volumes of transaction data.

## 🎯 Project Objectives

- Build an end-to-end cloud-based data engineering workflow.
- Store transaction data using Azure Data Lake Storage Gen2.
- Automate pipeline execution using Azure Data Factory.
- Process and transform data using Azure Databricks and PySpark.
- Implement Bronze, Silver and Gold data layers.
- Store curated data in Azure SQL Database.
- Visualise transaction insights using Power BI.
- Understand data quality, validation and pipeline monitoring.

---

## 🏗️ System Architecture

The project follows this processing workflow:

```text
       Python
          |
          v
   Source Transaction Data
          |
          v
 Azure Data Lake Storage Gen2
          |
          v
    Azure Data Factory
          |
          v
   Azure Databricks
          |
          v
    Bronze Layer
          |
          v
    Silver Layer
          |
          v
     Gold Layer
          |
          v
   Azure SQL Database
          |
          v
       Power BI
          |
          v
   Interactive Dashboard
```

## ⚙️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Source data preparation |
| PySpark | Distributed data processing |
| Azure Data Lake Storage Gen2 | Cloud data storage |
| Azure Data Factory | Pipeline orchestration |
| Azure Databricks | Data transformation |
| Delta Lake | Reliable data storage |
| Azure SQL Database | Structured data serving |
| Power BI | Data visualisation |

---

## 🥉 Medallion Architecture

The project uses three processing layers.

### 1. Bronze Layer

The Bronze layer stores incoming transaction records with minimal modifications.

**Purpose:**
- Preserve source transaction information.
- Maintain an initial processed copy of the data.
- Support data tracing and reprocessing.

### 2. Silver Layer

The Silver layer focuses on data cleaning and standardisation.

**Operations include:**
- Handling missing values.
- Removing duplicate records.
- Standardising data types.
- Validating important fields.
- Preparing consistent transaction records.

### 3. Gold Layer

The Gold layer contains curated, reporting-ready information.

**Purpose:**
- Prepare transaction-level outputs.
- Generate analytical summaries.
- Organise information for SQL queries.
- Support Power BI dashboards and reporting.

---

## 🔄 Project Workflow

1. **Data Preparation:** Prepare transaction records using Python.
2. **Data Ingestion:** Upload source files to Azure Data Lake Storage Gen2.
3. **Bronze Processing:** Ingest and retain source transaction records.
4. **Silver Processing:** Clean, validate and standardise transaction data.
5. **Gold Processing:** Generate curated datasets and analytical summaries.
6. **Database Integration:** Load prepared outputs into Azure SQL Database.
7. **Visualisation:** Connect Power BI to the prepared data and create dashboards.

---

## 📊 Power BI Dashboard

The Power BI dashboard provides a visual overview of transaction information.

The dashboard includes:

- Total Transactions
- Flagged Transactions
- Fraud Percentage
- Average Transaction Amount
- Transaction Analysis by City
- Merchant Category Analysis
- Merchant-wise Transaction Analysis
- Time-based Transaction Analysis

The dashboard helps users explore transaction patterns through graphical representations and filters.

**Note:** The fraud indicators in this training project are demonstration indicators. They are not independently validated fraud predictions or confirmed banking fraud outcomes.

---

## 🛠️ Data Quality and Validation

Data quality is an important part of the pipeline.

The following validation activities are considered:

- Checking source files and required columns.
- Identifying duplicate transaction identifiers.
- Validating transaction amounts and timestamps.
- Checking missing or invalid values.
- Comparing record counts across processing layers.
- Reconciling Gold-level summaries with SQL queries.
- Verifying Power BI dashboard results.

---

## 📁 Suggested Repository Structure

```text
Credit-Card-Fraud-Detection-Pipeline/
│
├── README.md
│
├── Report/
│   └── Industrial_Training_Report.pdf
│
├── Architecture/
│   └── System_Architecture.png
│
├── Screenshots/
│   ├── Azure_Storage.png
│   ├── Azure_Databricks.png
│   ├── Azure_Data_Factory.png
│   ├── SQL_Connection.png
│   └── PowerBI_Dashboard.png
│
├── Notebooks/
│   ├── Bronze/
│   ├── Silver/
│   └── Gold/
│
├── Datasets/
│
├── SQL/
│
└── PowerBI/
    └── Dashboard.pbix
```

*This is a suggested organisation for GitHub. Include only the folders and files that are actually available in your repository.*

---

## 🚀 Future Enhancements

The project can be extended with the following improvements:

- Real-time transaction processing using streaming technologies.
- Machine learning models for fraud classification.
- Improved pipeline monitoring and failure alerts.
- Incremental data loading and automated batch processing.
- Stronger data security and access management.
- Advanced Power BI dashboards and analytical reports.
- Model evaluation using Precision, Recall and F1-score.

---

## 🎓 Learning Outcomes

Through this project, I gained practical exposure to:

- Cloud-based data engineering concepts.
- Azure cloud services and resource management.
- Data pipeline development and orchestration.
- Apache Spark and PySpark transformations.
- Medallion Architecture.
- Delta Lake and structured data storage.
- SQL database integration.
- Power BI dashboard development.
- Data quality and validation techniques.

---

## 👨‍💻 Author

**Pankaj Johar**

- Degree: B.Tech – Computer Science & Engineering (AI)
- Institution: Swami Keshvanand Institute of Technology, Management & Gramothan, Jaipur
- Training Programme: Data Engineering with Python, Azure Databricks and Power BI
- Training Organisation: Coplur Technologies
- Session: 2026–27

---

## 📚 References

- Microsoft Learn – Azure Data Lake Storage Gen2
- Microsoft Learn – Azure Data Factory
- Microsoft Learn – Azure Databricks
- Apache Spark – PySpark Documentation
- Delta Lake Documentation
- Microsoft Learn – Power BI
- Microsoft Learn – Azure SQL Database

---

## 📄 Disclaimer

This project was developed as part of an academic industrial training programme. It demonstrates a learning-oriented data engineering pipeline and reporting workflow.

The fraud indicators and dashboard values are intended for demonstration purposes only. The project is not a production banking fraud detection system and does not claim independently verified fraud prediction accuracy.

---

**⭐ If you find this project useful, consider giving this repository a star!**
