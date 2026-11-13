# House Prices – Advanced Regression Techniques

A machine learning project based on Kaggle's **House Prices: Advanced Regression Techniques** competition. The goal is to predict residential property sale prices using regression models and feature engineering.

## Project Overview

This project explores the end-to-end workflow of a regression problem, including exploratory data analysis, preprocessing, feature engineering, feature selection, model evaluation, and Kaggle submission.

## Dataset

The dataset is provided by the [Kaggle House Prices competition](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques).

- Training data: 1,460 observations
- Test data: 1,459 observations
- Target variable: `SalePrice`

Download the competition data and place the CSV files in the `data/` directory.

## Methods and Techniques

- Exploratory Data Analysis
- Missing Value Imputation
- One-Hot Encoding and Ordinal Encoding
- Feature Selection
  - Mutual Information
  - SelectFromModel
  - Sequential Feature Selection
  - Variance Threshold
- Pearson and Spearman Correlation Analysis
- Variance Inflation Factor (VIF)
- Cyclical Feature Engineering
- Log Transformation of the Target Variable

## Models

The following regression models were evaluated:

- Ridge Regression
- Random Forest Regressor

Models were compared using 5-fold cross-validation and Root Mean Squared Logarithmic Error (RMSLE).

## Results

| Model | Cross-Validation RMSLE |
|---|---:|
| Ridge Regression | 0.148215 |
| Random Forest | **0.143184** |

Random Forest achieved the best cross-validation result.

**Kaggle Public Score:** 0.14437

## Repository Structure

```text
.
├── data/
├── tests/
├── houses_kaggle_competition.ipynb
├── README.md
├── requirements.txt
├── .gitignore
└── Makefile
```

## How to Run

1. Clone the repository.
2. Install the required dependencies.
3. Download the competition dataset and place the CSV files in `data/`.
4. Open `houses_kaggle_competition.ipynb`.
5. Run the notebook cells in order.

## Acknowledgements

Dataset and project assignment: Workintech Data Science Training Program.

Competition: [Kaggle – House Prices](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)
