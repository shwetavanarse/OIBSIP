# 🎯 Customer Segmentation Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![ML](https://img.shields.io/badge/ML-KMeans%20Clustering-orange.svg)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen.svg)

## 📌 Project Overview

This project applies **K-Means clustering** to segment an e-commerce company's customer base using **RFM analysis (Recency, Frequency, Monetary)** — a proven framework for understanding customer value and behavior. The goal is to identify distinct customer groups to enable targeted marketing strategies.

Completed as part of the **Oasis Infobyte Data Analytics Internship (OIBSIP)**.

---

## 🎯 Objective

To segment customers into meaningful groups based on purchasing behavior, enabling the business to tailor marketing strategies — from re-engagement campaigns to VIP retention programs.

---

## 🗂️ Dataset

**Source:** [Online Retail Dataset](https://archive.ics.uci.edu/dataset/352/online+retail) (UCI / Kaggle)

| Detail | Value |
|---|---|
| Original Rows | 141,049 |
| Rows After Cleaning | ~96,000+ |
| Key Columns Used | InvoiceNo, InvoiceDate, Quantity, UnitPrice, CustomerID |

**Cleaning steps:** Removed rows with missing CustomerID, excluded cancelled orders (negative quantity), removed invalid prices, and engineered a `TotalPrice` feature.

---

## 🛠️ Tools & Libraries

- **Python 3**
- **pandas** — data manipulation
- **scikit-learn** — StandardScaler, KMeans
- **matplotlib** & **seaborn** — visualization
- **Google Colab / Jupyter Notebook**

---

## 🔍 Methodology

1. **Data Cleaning** — removed unidentified customers and invalid transactions
2. **RFM Feature Engineering**:
   - **Recency** — days since last purchase
   - **Frequency** — number of unique orders
   - **Monetary** — total amount spent
3. **Standardization** — scaled RFM values using StandardScaler (required for distance-based clustering)
4. **Elbow Method** — determined optimal number of clusters
5. **K-Means Clustering** — applied with K=4
6. **Cluster Profiling** — calculated average R, F, M per cluster and interpreted business meaning
7. **Visualization** — scatter plots (Recency vs Monetary, Frequency vs Monetary) and cluster size distribution

---

## 💡 Customer Segments Identified

| Cluster | Segment Name | Recency (days) | Frequency | Monetary | Count |
|---|---|---|---|---|---|
| 0 | **At Risk / Inactive** | 89.6 | 1.3 | $462.5 | 760 |
| 1 | **Regular Customers** | 22.5 | 2.4 | $924.8 | 1,341 |
| 2 | **VIP Whales** | 22.2 | 8.0 | $51,546.8 | 6 |
| 3 | **Loyal High-Frequency Buyers** | 10.6 | 23.9 | $13,786.1 | 20 |

---

## 📈 Marketing Recommendations

- **At Risk (Cluster 0)** → Win-back campaigns with targeted discounts to prevent churn
- **Regular (Cluster 1)** → Loyalty points and bundle offers to increase order value
- **VIP Whales (Cluster 2)** → Dedicated account management and exclusive early access — protect this segment at all costs
- **Loyal High-Frequency (Cluster 3)** → Formal VIP/referral program to reward and retain engagement

---

## 📁 Repository Structure
DataAnalytics-L1-CustomerSegmentation/
├── README.md
├── Customer_Segmentation.ipynb
└── online_retail.csv


---

## 🚀 How to Run

1. Clone this repository or download the notebook
2. Open `Customer_Segmentation.ipynb` in Jupyter Notebook or Google Colab
3. Ensure `online_retail.csv` is in the same directory
4. Run all cells sequentially

---

## 🙌 Acknowledgment

This project was completed as part of the **Oasis Infobyte Summer Internship Program (OIBSIP)** — Data Analytics Track.

---

*Author: [Shweta Vanarse] | Internship: Oasis Infobyte | Track: Data Analytics*
