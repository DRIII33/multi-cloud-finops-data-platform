# Multi-Cloud FinOps Data Platform: Cloudability-Inspired Cost & Utilization Strategy System

## 📌 Project Overview
**Role Alignment:** Senior Data Strategist, IBM Cloudability (Austin/Boston/Bellevue)
**Context:** December 2025

This project simulates the core data engine of a modern FinOps platform. It ingests raw billing data from AWS, Azure, and GCP, normalizes it to the **FinOps Open Cost & Usage Specification (FOCUS) v1.0**, and prepares it for high-performance analytics in BigQuery. The platform addresses key challenges facing IBM Cloudability in 2025: unifying multi-cloud schemas, ensuring data quality at scale, and powering AI-driven optimization recommendations.

## 🏗️ Architecture
**Ingestion (Python/Pandas)** → **Normalization (FOCUS Schema)** → **Data Warehouse (BigQuery)** → **AI/ML Layer (Isolation Forest/Prophet)** → **BI Layer (Looker Studio)**

## 🛠️ Tools Used
* **Python 3.10+**: Data processing, validation, and ML.
* **Pandas**: In-memory manipulation.
* **BigQuery**: Serverless data warehousing.
* **Scikit-Learn**: Anomaly detection.
* **Prophet**: Cost forecasting.
* **FOCUS Schema**: Industry standard for billing normalization.

## 🚀 Key Features
1.  **Synthetic Data Engine:** Includes data_generator.py which algorithmically creates 90 days of hourly/daily billing data. It simulates weekend seasonality, resource drift, and injected cost spikes to rigorously test the Anomaly Detection and Forecasting modules.
2.  **FOCUS Normalization:** Unifies AWS `lineItem/ProductCode`, Azure `MeterCategory`, and GCP `Service Description` into a single semantic layer.
3.  **Automated Data Quality:** 40+ checks for nulls, drift, and schema violations.
4.  **Cost Optimization:** SQL models that identify idle RDS instances, unattached EBS volumes, and rightsizing opportunities.
5.  **AI Integration:** Python-based anomaly detection pipeline to flag spend spikes before the invoice arrives.

   g modules.

## 📋 Repository Structure
* `/data/`: Synthetic datasets mimicking real cloud billing exports.
* `/python_scripts/`: Modular ETL and ML scripts.
* `/bigquery_sql/`: Dimensional modeling and BI view generation.
* `/documentation/`: Strategic documents aligning with IBM's 2025 roadmap.

## 💡 Key Takeaway for Recruiters
This project demonstrates the ability to translate ambiguous multi-cloud data problems into a structured, scalable data strategy—exactly what is required to lead data architecture at IBM Cloudability.
