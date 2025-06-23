# Large Scale Retail Data Analysis (32 Million Records) | Python | Fireducks | Pandas

## Overview
This project demonstrates scalable data analysis techniques applied to a massive dataset with over 32 million records. Using modern Python libraries like `fireducks` (DuckDB-based), we perform memory-optimized data cleaning, exploratory data analysis (EDA), and preliminary statistical insights — all in a way that can scale far beyond what standard pandas workflows handle.

## Table of Contents
- [Overview](#overview)
- [Project Description](#project-description)
- [Data](#data)
- [Methodology](#methodology)
- [Analysis and Findings](#analysis-and-findings)
- [Recommendations](#recommendations)
- [Ad Hoc Use Cases](#ad-hoc-use-cases)
- [Files and Resources](#files-and-resources)
- [Conclusion](#conclusion)
- [Acknowledgment](#acknowledgment)
- [Contact Information](#contact-information)

## Project Description

### Background
With the explosion of data volume in modern organizations, traditional pandas operations often fail to scale — either due to memory limits or sluggish performance. This project explores a high-performance, notebook-based analysis approach using DuckDB-powered `fireducks.pandas` to overcome these limitations and process Excel/CSV files containing tens of millions of rows.

### Objective
- Efficiently handle and preprocess 32M+ records.
- Leverage DuckDB's power via Fireducks for fast I/O and operations.
- Analyze distributions, patterns, and anomalies in real-world datasets.
- Serve as a scalable, reproducible analytics template for large tabular data.

## Data

### Data Source
The data used in this project is assumed to be a large structured CSV/Excel file comprising transactional records or observational data. Specifics have been kept generic for privacy and reproducibility.

### Data Description
- **Date Columns:** Timestamps for events or records
- **Categorical Columns:** Product, location, status, etc.
- **Numerical Columns:** Quantities, costs, profits
- **Missing/Nulls:** Real-world messiness requiring imputation and cleaning

## Methodology

### Approach
- **Fireducks Integration:** Load and process massive data files without RAM choke points.
- **Data Cleaning:** Handle missing values, drop irrelevant features, format columns.
- **Type Optimization:** Convert datatypes to reduce memory usage (e.g., `category`, `float32`)
- **Visualization:** Leverage matplotlib for EDA insights like frequency plots, trend lines.

### Tools and Technologies
- **Python 3.10+**
- **Pandas**
- **Fireducks (DuckDB integration)**
- **Matplotlib**

## Analysis and Findings

### Key Insights
- **Missing Data:** Identification and treatment strategies deployed on key columns.
- **Type Mismatches:** Converted object-heavy columns to numeric or categorical types.
- **EDA Outcomes:** Plotted distributions of major features, visualized outliers and frequency.
- **Performance:** Compared performance metrics between pandas and fireducks operations.

## Recommendations

### Scaling Strategy
- Move away from in-memory pandas workflows for files >10M rows.
- Prefer columnar storage (Parquet) + DuckDB/Polars for heavy workloads.
- Validate data cleaning logic with samples before applying across full dataset.

### Tooling Advice
- Use Fireducks for read-heavy and transformation-heavy operations.
- Integrate cloud-based notebooks (Colab, JupyterHub) when local memory is limited.

## Ad Hoc Use Cases
1. **Excel/CSV File > 1GB Ingestion**
2. **Exploratory Analysis on 30M+ Records**
3. **DuckDB Benchmarks vs Pandas**
4. **Memory Optimization Checklist**
5. **Large File Profiling Template**

## Files and Resources
- `Large_Scale_Data_Analysis.ipynb` – Full notebook with code and comments
- Dependencies: Listed via pip commands inside the notebook (`fireducks`, `pandas`, etc.)

## Conclusion
This project showcases how scalable analytics pipelines can be built using modern Python tools without requiring full-blown big data platforms. By leveraging `fireducks` and DuckDB, analysts can handle 10M+ records directly in notebooks with efficient memory and compute utilization.

## Acknowledgment
This project was conceptualized, developed, and maintained by **Adhithya Krishnan** as part of self-learning initiatives in handling large datasets. It aims to help other data professionals overcome pandas bottlenecks and adopt scalable workflows.

## Contact Information
For feedback, collaboration, or professional inquiries:

- [LinkedIn](https://www.linkedin.com/in/adhithyakrishnan)
- [Portfolio Website](https://adhithyakrishnanmp-portfolio-website.vercel.app/)
- [GitHub](https://github.com/Adhithyakrishnan)
