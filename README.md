# California Wine Production Analysis (1980–2020) 🍷

A machine learning project to analyze and predict wine grape production
across 42 counties in California over 40 years using regression models.

## Problem statement
California is the largest wine-producing state in the US. This project
analyzes historical wine grape production data from 1980 to 2020 and
builds regression models to predict production output based on
harvested acres, yield, price, and other agricultural factors.

## Dataset

| Feature | Description |
|---------|-------------|
| Year | 1980 – 2020 |
| County | 42 California counties |
| HarvestedAcres | Total acres harvested |
| Yield(Unit/Acre) | Yield per acre |
| Production | Total production in tons (target variable) |
| Price(Dollars/Unit) | Price per ton |
| Value(Dollars) | Total dollar value of production |
| CropName | Type of wine grape |
| Unit | Unit of measurement |

- **Total records:** 1,315
- **Source:** California Department of Food and Agriculture (CDFA)

## Project workflow

```
1. Data Loading & Exploration
2. Data Cleaning (null handling, unit standardization)
3. Feature Engineering (Label Encoding)
4. Train/Test Split (80/20)
5. Model Training & Evaluation
6. Comparison of 7 Regression Models
```

## Models used

| Model | Type |
|-------|------|
| Linear Regression | Baseline |
| Lasso Regression | Regularized Linear |
| Ridge Regression | Regularized Linear |
| Decision Tree Regressor | Tree-based |
| Random Forest Regressor | Ensemble |
| Support Vector Regression (SVR) | Kernel-based |
| K-Nearest Neighbors Regressor | Instance-based |

## Evaluation metrics
- **Mean Squared Error (MSE)**
- **R-squared (R²)**

## How to run

```bash
git clone https://github.com/Mokshitha08/<repo-name>
cd <repo-name>
pip install pandas scikit-learn matplotlib seaborn
```

Then open the notebook in Jupyter or Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Mokshitha08/)

## Tools & libraries

`Python` · `pandas` · `scikit-learn` · `matplotlib` · `seaborn` · `Jupyter Notebook`

## Key insights
- Wine grape production varies significantly across California counties
- Harvested acres and yield are the strongest predictors of production
- Ensemble models (Random Forest) outperform linear models on this dataset
- Prices have increased significantly from 1980 to 2020
