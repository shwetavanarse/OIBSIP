# 📊 Exploratory Data Analysis on Retail Sales Data

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458.svg)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen.svg)

## 📌 Project Overview

This project performs a comprehensive **Exploratory Data Analysis (EDA)** on the Superstore retail sales dataset to uncover meaningful patterns in sales performance, customer behavior, and profitability. The goal is to translate raw transactional data into **actionable business insights** that can guide strategic decisions around discounting, inventory, and customer targeting.

This task was completed as part of the **Oasis Infobyte Data Analytics Internship (OIBSIP)**.

---

## 🎯 Objective

To explore a real-world retail dataset and answer key business questions:
- How do sales trend over time?
- Which products and categories drive the most revenue?
- Who are our customers, and how do they differ?
- Does discounting help or hurt profitability?

---

## 🗂️ Dataset

**Source:** [Sample Superstore Dataset](https://www.kaggle.com/datasets) (Kaggle)

| Detail | Description |
|---|---|
| Rows | 9,994 |
| Columns | 21 |
| Time Range | Jan 2014 – Dec 2017 |
| Missing Values | None |

Key columns: `Order Date`, `Sales`, `Profit`, `Discount`, `Quantity`, `Category`, `Sub-Category`, `Region`, `Segment`

---

## 🛠️ Tools & Libraries

- **Python 3**
- **pandas** — data manipulation
- **matplotlib** & **seaborn** — data visualization
- **Google Colab / Jupyter Notebook** — development environment

---

## 🔍 Analysis Performed

1. **Data Inspection** — shape, data types, null value checks
2. **Descriptive Statistics** — mean, median, std deviation across numerical fields
3. **Time Series Analysis** — monthly & quarterly sales trends
4. **Customer Segment Analysis** — order distribution across Consumer, Corporate, and Home Office segments
5. **Product Performance** — top 10 best-selling products by revenue
6. **Category Analysis** — revenue breakdown by product category
7. **Correlation Analysis** — heatmap of Sales, Quantity, Discount, and Profit
8. **Discount Impact Analysis** — scatter plot examining the relationship between discount levels and profitability

---

## 💡 Key Insights

- 📈 **Seasonal spikes**: Sales consistently peak in **November and December** each year, driven by holiday shopping.
- 👥 **Customer segments**: The **Consumer** segment accounts for the highest order volume, ahead of Corporate and Home Office.
- 🏆 **Top categories**: **Technology** and **Furniture** generate the highest total revenue.
- ⚠️ **Discounting hurts profit**: Discount and Profit show a **negative correlation (-0.22)**. Orders discounted above **~40%** frequently result in a **net loss**, as shown clearly in the scatter plot analysis.

---

## 📈 Business Recommendations

1. **Cap standard discounts at 20–30%**, requiring approval for anything higher, to protect profit margins.
2. **Prioritize Technology and Furniture** in Q4 promotional campaigns, aligning with existing seasonal demand.
3. **Build loyalty programs targeted at the Consumer segment**, since they represent the largest share of orders.
4. **Audit high-discount, low-profit products** individually to identify pricing issues beyond discounting alone.

---

## 📁 Repository Structure
DataAnalytics-L1-EDARetailSales/
├── README.md
├── EDA_Retail_Sales.ipynb
└── sample_-_superstore.csv


---

## 🚀 How to Run

1. Clone this repository or download the notebook
2. Open `EDA_Retail_Sales.ipynb` in Jupyter Notebook or Google Colab
3. Ensure `sample_-_superstore.csv` is in the same directory (or update the file path)
4. Run all cells sequentially

---

## 🙌 Acknowledgment

This project was completed as part of the **Oasis Infobyte Summer Internship Program (OIBSIP)** — Data Analytics Track.

---

*Author: [Shweta Vanarse] | Internship: Oasis Infobyte | Track: Data Analytics*
