# 🧹 Data Cleaning & Preprocessing Pipeline

[![Python](https://img.shields.io/badge/Python-3.9+-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Wrangling-150458?style=flat&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-Computation-013243?style=flat&logo=numpy&logoColor=white)](https://numpy.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=flat&logo=jupyter&logoColor=white)](https://jupyter.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 📌 Project Overview

In real-world scenarios, raw data is rarely analysis-ready. It often contains inconsistencies, missing values, duplicates, and structural anomalies. 

This project demonstrates an **end-to-end data cleaning and preprocessing pipeline** using Python. The objective is to transform raw, unstructured/messy data into a robust, high-integrity dataset optimized for **Exploratory Data Analysis (EDA)**, **Business Intelligence dashboards**, and downstream **Machine Learning workflows**.

---

## 🛠️ Tech Stack & Libraries

1. **Data Ingestion & Structural Inspection:**
   - Evaluated data schemas, missingness patterns, and statistical distributions using `.info()`, `.describe()`, and `.isna().sum()`.
2. **Missing Data Imputation & Handling:**
   - Analyzed MCAR/MAR/MNAR patterns. Applied context-aware strategies (median for skewed metrics, mode for categorical features, or row dropping where appropriate).
3. **Deduplication & Integrity Verification:**
   - Identified and purged duplicate records to prevent bias and skewed aggregate metrics.
4. **Schema Standardization & Type Casting:**
   - Standardized column names using `snake_case`. Converted string timestamps into proper `datetime64` objects and normalized categorical entries.
5. **Outlier Detection & Treatment:**
   - Identified anomalous values via IQR (Interquartile Range) filtering and distribution plots (boxplots/histograms).
6. **Data Export:**
   - Exported the sanitized dataset into optimized formats (`.csv` / `.parquet`) for subsequent analytical phases.

---

## 📁 Repository Structure
```text
├── data set/
│   ├── data/                 # Original, immutable raw dataset│   
├── Data_Cleaning.ipynb       # Step-by-step cleaning walkthrough
├── requirements.txt          # Reproducible environment dependencies
└── README.md                 # Project documentation


## ⚙️ Key Preprocessing Steps
