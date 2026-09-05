# 🧹 Data Cleaning — Titanic Dataset

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Cleaning-150458.svg)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen.svg)

## 📌 Project Overview

This project demonstrates professional-level data cleaning by taking the classic **Titanic dataset** — a deliberately messy, real-world dataset — and systematically transforming it into a clean, analysis-ready dataset. Every cleaning decision is documented and justified.

Completed as part of the **Oasis Infobyte Data Analytics Internship (OIBSIP)**.

---

## 🎯 Objective

To take raw, messy data and produce a clean dataset suitable for downstream analysis or machine learning, while documenting the reasoning behind every cleaning decision.

---

## 🗂️ Dataset

**Source:** [Titanic Dataset](https://www.kaggle.com/c/titanic) (Kaggle)

| Detail | Value |
|---|---|
| Original Rows | 891 |
| Original Columns | 12 |
| Missing Data | Age (19.87%), Cabin (77.10%), Embarked (0.22%) |
| Duplicates | 0 |

---

## 🛠️ Tools & Libraries

- **Python 3**
- **pandas** — data cleaning & manipulation
- **numpy** — numerical operations
- **Google Colab / Jupyter Notebook**

---

## 🔍 Cleaning Process

1. **Data Quality Report** — audited nulls, duplicates, and data types before touching anything
2. **Missing Data Handling**:
   - `Age` → filled with **median** (robust to outliers/skew)
   - `Embarked` → filled with **mode** (only 2 rows affected)
   - `Cabin` → **dropped** (77% missing — unreliable for imputation)
3. **Duplicate Removal** — confirmed and removed 0 duplicate rows
4. **Standardization** — verified `Sex` and `Embarked` had consistent formatting (no case mismatches)
5. **Outlier Detection** — used the **IQR method** on `Fare`; found 116 outliers, **retained** them as legitimate high-fare passengers rather than data errors
6. **Data Type Correction** — converted `PassengerId` to string (it's an identifier, not a quantity)
7. **Before vs After Summary** — documented every change in a comparison table
8. **Exported** the final cleaned dataset as `titanic_cleaned.csv`

---

## 💡 Key Decisions & Justifications

| Column | Issue | Decision | Reasoning |
|---|---|---|---|
| Age | 19.87% missing | Filled with median | Robust to skew from outlier ages |
| Embarked | 0.22% missing | Filled with mode | Minimal impact, only 2 rows |
| Cabin | 77.10% missing | Dropped column | Too sparse to impute reliably |
| Fare | 116 outliers (IQR) | Retained | Reflects real 1st-class pricing, not errors |

---

## 📁 Repository Structure
DataAnalytics-L1-CleaningData/
├── README.md
├── Cleaning_Data_Titanic.ipynb
├── train.csv
└── titanic_cleaned.csv


---

## 🚀 How to Run

1. Clone this repository or download the notebook
2. Open `Cleaning_Data_Titanic.ipynb` in Jupyter Notebook or Google Colab
3. Ensure `train.csv` is in the same directory
4. Run all cells sequentially to reproduce the cleaning pipeline
5. Output: `titanic_cleaned.csv` — the fully cleaned dataset

---

## 🙌 Acknowledgment

This project was completed as part of the **Oasis Infobyte Summer Internship Program (OIBSIP)** — Data Analytics Track.

---

*Author: [Shweta Vanarse] | Internship: Oasis Infobyte | Track: Data Analytics*
