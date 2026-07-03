# Advanced Apex Project

## Manufacturing: Autonomous Maintenance Assistant Pipeline

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)]()
[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)]()
[![BITS Pilani](https://img.shields.io/badge/BITS%20Pilani-Advanced%20Apex%20Project-success.svg)]()

---

## Project Overview

This repository contains my **Advanced Apex Project** developed as part of the **BITS Pilani BS Programme**.

The project focuses on designing and implementing a **complete manufacturing data preprocessing pipeline** for predictive maintenance using the **NASA CMAPSS FD001** dataset.

Rather than training a machine learning model, the objective is to prepare high-quality manufacturing sensor data by applying data cleaning, preprocessing, feature engineering, quality validation, and exploratory analysis to generate structured datasets suitable for downstream predictive maintenance applications.

---

## Problem Statement
P3

**Manufacturing: Autonomous Maintenance Assistant Pipeline**

**Problem Statement Description** 

Manufacturing plants collect sensor readings, production line states, operator notes, and maintenance records from machines. Your task is to build a data pipeline that prepares this raw data for an autonomous maintenance assistant. The dataset will contain timestamp gaps, noisy spikes, missing sensor readings, inconsistent machine identifiers, and uneven sampling rates. The goal is to create a clean time aligned feature table that helps identify early patterns before maintenance events or machine faults.

**Brief Description**

• Ingest machine sensor logs, production line status data, and maintenance records.

• Clean machine identifiers and align sensor readings with timestamps.

• Handle missing samples through clear rules such as interpolation or removal of long gaps.

• Detect and treat impossible spikes in temperature, vibration, current, or pressure values.

• Normalize sensor values per machine and create fixed time window summaries.

• Create a simple output such as sensor trends before maintenance or correlation among vibration, temperature, and fault events.

• Time series preprocessing

• Data integration

• Resampling

• Outlier detection

• Feature engineering

• Before and after data quality reporting

• AI4I 2020 Predictive Maintenance dataset

• NASA Turbofan Engine Degradation dataset

• UCI SECOM manufacturing dataset

• Hydraulic System Condition Monitoring dataset

So, Manufacturing plants continuously generate sensor readings, production states and maintenance records from industrial equipment.

**Raw manufacturing data often contains:**

- Missing observations
- Noisy sensor measurements
- Outliers
- Inconsistent identifiers
- Uneven time-series records

This project develops a robust preprocessing pipeline that transforms raw industrial sensor data into clean, structured feature tables for future predictive maintenance systems.

---

## Dataset

**Primary Dataset**

NASA Commercial Modular Aero-Propulsion System Simulation (CMAPSS)
https://data.nasa.gov/dataset/cmapss-jet-engine-simulated-data

Dataset Used:

- FD001

Dataset Characteristics

- 20,631 observations
- 26 columns
- 100 engines
- 21 sensor measurements
- Time-series degradation data

---

## Project Pipeline

The notebook implements the following preprocessing pipeline:

1. Dataset Loading
2. Dataset Inspection
3. Data Quality Assessment
4. Time-Series Preparation
5. Machine Identifier Validation
6. Missing Value Handling
7. Sensor Normalisation
8. Outlier Detection
9. Outlier Treatment
10. Feature Engineering
11. Remaining Useful Life (RUL)
12. Engine Health Index
13. Maintenance Risk Classification
14. Correlation Analysis
15. Sensor Trend Analysis
16. Pipeline Validation
17. Before & After Data Quality Reporting
18. Export of Processed Datasets

---

## Feature Engineering

The project generates several useful features including:

- Remaining Useful Life (RUL)
- Rolling Mean
- Rolling Standard Deviation
- Rate of Change
- Fixed Window Statistics
- Engine Health Index
- Maintenance Risk Classification
- Engine Summary Table

---

## Outputs

The pipeline exports:

- Clean Sensor Dataset
- Engine Feature Table
- Engine Summary
- Before & After Data Quality Report

---

## Repository Structure

```text
Advanced-Apex-Project/
│
├── CMAPSSData/
│   └── train_FD001.txt
│
├── Pipeline_Implimentation.ipynb
├── Project_Outline.docx
├── Final_Project_Report.docx
├── GenAI_Prompt_Log.docx
│
└── README.md
```

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Google Colab

---

## Learning Outcomes

This project demonstrates practical implementation of:

- Industrial Data Preprocessing
- Time-Series Data Processing
- Manufacturing Analytics
- Feature Engineering
- Data Quality Assessment
- Exploratory Data Analysis
- Predictive Maintenance Data Preparation

---

## Future Scope

Potential future enhancements include:

- Remaining Useful Life prediction
- Predictive maintenance models
- Real-time Industrial IoT integration
- Streaming data pipelines
- Interactive dashboards
- Cloud deployment

---

## Author

**Sai Spoorthy Eturu**

BITS Pilani BS Programme

Advanced Apex Project

GitHub: https://github.com/ESpoorthy

---

## Acknowledgements

- BITS Pilani BS Programme
- NASA Prognostics Center of Excellence
- Python Open Source Community
