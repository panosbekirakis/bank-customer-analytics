# Bank Customer Analytics

## Project Overview
Exploratory Data Analysis and Feature Selection for predicting bank customer churn.
A bank wants to identify which customers are likely to leave so targeted retention 
strategies can be applied proactively.

## Dataset
- **File:** `bank_customer_analytics.csv`
- **Rows:** 3,000 customers
- **Columns:** 12 (6 numerical + 5 categorical + 1 target)
- **Target:** `churn` — yes (customer left) / no (customer stayed)
- **Class balance:** 69.8% stayed · 30.2% churned

## EDA Pipeline (11 Steps)
1. Understand the Problem
2. Load and Inspect the Dataset
3. Handle Missing Values (KNN Imputation + Median comparison + Flag columns)
4. Rename Columns
5. Check and Fix Data Types
6. Value Counts per Column
7. Univariate Analysis + Variance Thresholding
8. Outlier Detection (Boxplots + IQR + Scatterplots)
9. Bivariate & Multivariate Analysis (Boxplots + Grouped Bar Plots + Pairplot)
10. Correlation Analysis (Pearson + Information Gain + Random Forest + RFE + Gradient Boosting)
11. Domain-Specific Feature Understanding

## Feature Selection
Two final datasets produced:
- **Option 1:** All 10 features kept
- **Option 2:** gender and loanstatus dropped (weakest across all 5 methods)

## How to Run
1. Clone or download this repository
2. Place `bank_customer_analytics.csv` in the same folder as the notebook
3. Open `Python Project_bank_customer_analytics.ipynb` in Jupyter Notebook
4. Run all cells — final CSV files will be generated automatically

## Tools & Libraries
- **Language:** Python 3
- **Environment:** Jupyter Notebook
- **Libraries:** pandas · numpy · matplotlib · seaborn · scikit-learn

## Author
Panos Bekirakis
