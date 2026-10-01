**SUPERMARKET SALES STRATEGY RECOMENDATION**

## 📌 Project Overview

This project analyzes supermarket transaction data to identify **customer segments** and **purchasing patterns** that can be translated into targeted sales strategies.

The project combines:

- **RFM Analysis** to understand customer purchasing behavior
- **K-Means Clustering** to segment customers based on their Recency, Frequency, and Monetary values
- **FP-Growth** to identify products that are frequently purchased together within each customer segment
- **Association Rule Analysis** using Support, Confidence, and Lift
- **Business Strategy Development** based on customer characteristics and product associations

The main objective is to move beyond general marketing strategies by developing recommendations that are tailored to the purchasing behavior of different customer segments.

---

## 🎯 Objectives

The project aims to:

1. Segment customers based on their purchasing behavior using RFM and K-Means.
2. Identify frequently purchased product combinations within each customer segment using FP-Growth.
3. Evaluate association rules using Support, Confidence, and Lift.
4. Translate analytical findings into segment-specific sales strategies.

---

## 📊 Dataset

The dataset contains historical transaction records from a supermarket in France covering **December 2010 to December 2011**.

The dataset consists of **8,557 transaction records** with the following attributes:

| Feature | Description |
|---|---|
| `InvoiceNo` | Transaction/invoice number |
| `StockCode` | Product code |
| `Product` | Product description |
| `Quantity` | Number of products purchased |
| `InvoiceDate` | Transaction date and time |
| `UnitPrice` | Price per product |
| `CustomerID` | Customer identifier |
| `Country` | Customer's country |

The dataset was obtained from a public dataset available on [Kaggle](https://www.kaggle.com/datasets/carrie1/ecommerce-data).
From the original dataset, this project specifically uses transaction data from **France** only, covering the period from **December 2010 to December 2011**.

---

## 🔍 Methodology

The overall workflow consists of the following stages:

```text
Raw Transaction Data
        ↓
Exploratory Data Analysis
        ↓
Data Preprocessing
        ↓
Product Aggregation & Filtering
        ↓
RFM Calculation
        ↓
RFM Normalization
        ↓
K-Means Customer Segmentation
        ↓
Transaction Separation by Cluster
        ↓
FP-Growth per Customer Segment
        ↓
Association Rule Evaluation
        ↓
Top Rules Based on Lift
        ↓
Sales Strategy Recommendation
