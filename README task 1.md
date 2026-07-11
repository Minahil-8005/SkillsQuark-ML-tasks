# Task 1: Data Cleaning & Exploratory Data Analysis (EDA) 🏠

Cleaning and exploring the **House Prices** dataset — handling missing values, encoding categorical features, removing outliers, and visualizing key relationships before building predictive models.

## 📋 Project Overview

This project performs a full data cleaning and EDA pipeline on the Kaggle **House Prices: Advanced Regression Techniques** dataset, preparing it for future regression modeling.

## 📊 Dataset

- **Source**: [Kaggle - House Prices: Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data)
- **File used**: `train.csv`
- **Target variable**: `SalePrice`
.

## 🛠️ Tech Stack

- Python 3.10+
- Pandas / NumPy
- Matplotlib / Seaborn
- Scikit-Learn (LabelEncoder, StandardScaler)
- Jupyter Notebook

## 📁 Project Structure

```
├── Task1_Data_Cleaning_EDA_HousePrices.ipynb   # Main notebook
├── requirements.txt                             # Python dependencies
├── .gitignore
└── README.md
```

## 🚀 How to Run

1. Clone this repository
```bash
git clone <your-repo-url>
cd <your-repo-name>
```

2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Download `train.csv` from Kaggle and place it in the project folder

4. Launch Jupyter Notebook
```bash
jupyter notebook
```

5. Open `Task1_Data_Cleaning_EDA_HousePrices.ipynb` and run all cells

## 📈 Workflow

1. **Data Loading** — Load `train.csv`, inspect shape and structure
2. **Exploratory Data Analysis** —
   - SalePrice distribution
   - Correlation heatmap
   - Living area vs Sale price
   - Outlier visualization (boxplots)
   - Overall quality vs Sale price
   - Missing values overview
3. **Data Cleaning** —
   - Fill categorical NaNs with `'None'` where the feature doesn't exist (e.g. no pool, no fence)
   - Fill numeric NaNs with `0` where applicable (e.g. no garage → GarageYrBlt = 0)
   - Fill `LotFrontage` using neighborhood-wise median
   - Fill `Electrical` with mode
4. **Categorical Encoding** — Label Encoding for ordinal quality columns
5. **Outlier Removal** — Remove extreme `GrLivArea` outliers
6. **Feature Scaling** — Standardize key numeric columns
7. **Export** — Save cleaned dataset as `cleaned_house_prices.csv`

## ✅ Outcome

- Fully cleaned, encoded, and scaled dataset ready for regression modeling
- Clear understanding of feature relationships with `SalePrice`
- Reusable data-cleaning pipeline for similar tabular datasets


