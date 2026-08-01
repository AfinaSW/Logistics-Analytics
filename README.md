# 🚛 Logistics Analytics Platform

An end-to-end logistics analytics solution built with **Microsoft Fabric** and **Power BI**.

The project demonstrates how Microsoft Fabric can be used to build a unified analytics platform by integrating data engineering, ETL, semantic modeling, and business intelligence within a single environment.

The solution follows the **Medallion Architecture (Bronze → Silver → Gold)** and delivers executive-level insights through an interactive Power BI dashboard.

---

## 📌 Business Problem

Logistics companies generate large volumes of operational data from transportation, warehousing, and customer management systems. Without a structured analytics platform, decision-makers struggle to monitor operational performance, control transportation costs, and identify profitability drivers.

This project demonstrates how raw operational data can be transformed into reliable business insights using Microsoft Fabric.

The dashboard enables business users to answer questions such as:

- How is revenue changing over time?
- What are the main transportation cost drivers?
- Which customers generate the highest profit?
- Which delivery routes perform best?
- How do delays affect operational performance?

---

## 🏗 Solution Architecture

The solution was built as an end-to-end analytics platform using Microsoft Fabric.

### Data Flow

```
Data Sources
      │
      ▼
Lakehouse
      │
      ▼
Bronze Layer
      │
      ▼
Silver Layer
      │
      ▼
Gold Layer
      │
      ▼
Semantic Model
      │
      ▼
Power BI Dashboard
```

The complete ETL process is orchestrated through Microsoft Fabric Data Pipelines.

---

## ⚙️ Technology Stack

| Technology | Purpose |
|------------|---------|
| Microsoft Fabric | Unified Analytics Platform |
| Lakehouse | Centralized Data Storage |
| Delta Lake | Data Format |
| PySpark | Data Transformation |
| SQL | Data Validation & Analysis |
| Data Pipeline | ETL Orchestration |
| Semantic Model | Business Layer |
| Power BI | Executive Dashboard |

---

## 🥉 Bronze Layer

The Bronze layer stores raw business data loaded into the Lakehouse.

No business transformations are applied at this stage.

---

## 🥈 Silver Layer

The Silver layer performs data cleansing and standardization.

Main transformations include:

- duplicate removal
- string standardization
- schema validation
- preparation for analytical processing

---

## 🥇 Gold Layer

The Gold layer contains business-ready analytical tables optimized for reporting.

Business calculations include:

- Revenue
- Transportation Cost
- Profit
- Profit Margin
- Cost Breakdown

These tables are consumed directly by the Semantic Model.

---

## 📊 Power BI Dashboard

The executive dashboard provides a consolidated view of logistics performance through three analytical pages:

### Executive Overview

- Revenue
- Profit
- Profit Margin
- Cost Breakdown
- Revenue Trend

### Operational Performance

- Route Performance
- Delivery Status
- Delay Analysis
- Cost Analysis

### Customer Analytics

- Customer Profitability
- Customer Revenue Ranking
- Customer Performance Metrics

---

## 📂 Repository Structure

```
📦 Logistics Analytics Platform
│
├── notebooks/
│   ├── 01_Bronze_Ingestion
│   ├── 02_Silver_Transformation
│   ├── 03_Gold_Delivery_Analytics
│   └── 04_Gold_Dimensions
│
├── pipeline/
│
├── semantic_model/
│
├── powerbi/
│
├── images/
│
└── README.md
```

---

## 🚀 Key Features

- End-to-end Microsoft Fabric solution
- Medallion Architecture
- Automated ETL Pipeline
- PySpark Data Transformation
- Delta Lake Storage
- Semantic Modeling
- Executive Power BI Dashboard
- Business KPI Monitoring


