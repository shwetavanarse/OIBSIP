# 🏠 Predicting House Prices with Linear Regression

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![ML](https://img.shields.io/badge/ML-Linear%20Regression-orange.svg)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen.svg)

## 📌 Project Overview

This project builds and evaluates a **Linear Regression model** to predict residential house sale prices using the Ames Housing dataset. The analysis covers the full machine learning workflow — from feature selection and encoding through to model evaluation and business interpretation of coefficients.

Completed as part of the **Oasis Infobyte Data Analytics Internship (OIBSIP)** — Level 2.

---

## 🎯 Objective

To build an interpretable regression model that accurately predicts house prices based on structural features and location, while identifying which factors most strongly influence value.

---

## 🗂️ Dataset

**Source:** [Ames Housing Dataset](https://www.kaggle.com/datasets) (Kaggle)

| Detail | Value |
|---|---|
| Rows | 2,930 |
| Original Columns | 82 |
| Selected Features | 9 numerical + Neighborhood (categorical) |
| Target Variable | `SalePrice` |

**Selected Features:** Gr Liv Area, Bedroom AbvGr, Full Bath, Overall Qual, Overall Cond, Year Built, Total Bsmt SF, Garage Cars, Lot Area, Neighborhood

---

## 🛠️ Tools & Libraries

- **Python 3**
- **pandas** — data manipulation
- **scikit-learn** — LinearRegression, train_test_split, evaluation metrics
- **matplotlib** & **seaborn** — visualization
- **Google Colab / Jupyter Notebook**

---

## 🔍 Methodology

1. **Feature Selection** — narrowed 82 columns down to 9 high-signal numerical features plus Neighborhood
2. **Missing Value Handling** — filled 2 minor gaps (Total Bsmt SF, Garage Cars) with median values
3. **Exploratory Analysis** — examined SalePrice distribution and feature correlations
4. **One-Hot Encoding** — converted the categorical `Neighborhood` column into dummy variables
5. **Train/Test Split** — 80/20 split
6. **Model Training** — fit a Linear Regression model
7. **Evaluation** — assessed using MSE, RMSE, and R²
8. **Diagnostics** — Actual vs Predicted scatter plot and residual analysis
9. **Coefficient Analysis** — interpreted which features drive price up or down

---

## 📊 Model Performance

| Metric | Value |
|---|---|
| **R² Score** | 0.8457 |
| **RMSE** | $35,177.33 |
| **MSE** | $1,237,444,680.75 |

The model explains **~84.6%** of the variation in house sale prices.

---

## 💡 Key Insights

- 📍 **Location dominates**: Neighborhood is the single strongest price driver — homes in **GrnHill, StoneBr, and NridgHt** command a **$60K–$112K premium** over baseline neighborhoods.
- 🏗️ **Age matters**: Each additional year of construction recency adds ~$472 to predicted price.
- 🛏️ **Counterintuitive bedroom effect**: Holding living area constant, more bedrooms slightly *decreases* predicted price — likely reflecting smaller, less desirable room sizes.
- 📈 **Model reliability**: Residuals are reasonably randomly distributed, though prediction accuracy decreases slightly for luxury-tier homes.

---

## 📁 Repository Structure
DataAnalytics-L2-HousePricePrediction/
├── README.md
├── House_Price_Prediction.ipynb
└── AmesHousing.csv

---

## 🚀 How to Run

1. Clone this repository or download the notebook
2. Open `House_Price_Prediction.ipynb` in Jupyter Notebook or Google Colab
3. Ensure `AmesHousing.csv` is in the same directory
4. Run all cells sequentially

---

## 🙌 Acknowledgment

This project was completed as part of the **Oasis Infobyte Summer Internship Program (OIBSIP)** — Data Analytics Track, Level 2.

---

*Author: [Shweta Vanarse] | Internship: Oasis Infobyte | Track: Data Analytics*
