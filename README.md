# Fraud Transaction EDA

## Project Overview

This project is an exploratory data analysis (EDA) of a credit card transaction dataset with the goal of understanding fraud patterns and preparing the data for further analytical and modeling tasks.

The dataset contains real-world anonymized financial transaction data and is commonly used for fraud detection research.  
The main focus of this project is:

- understanding the dataset structure
- exploring class imbalance
- analyzing transaction amount distribution
- comparing fraudulent and normal transactions
- practicing analytical thinking and data storytelling

---

## Project Goal

The goal of this project is to practice a full basic data analysis workflow using Python and Jupyter Notebook.

This includes:

- loading and inspecting a dataset
- checking data types and missing values
- identifying class imbalance
- exploring feature distributions
- interpreting results in a business and fraud-detection context

---

## Dataset

**Dataset name:** Credit Card Fraud Detection  
**Source:** Kaggle

The dataset contains credit card transactions made by European cardholders in September 2013.

### Notes about the data:
- transactions are anonymized
- most features are transformed with PCA and represents as `V1` to `V28`
- `Time` and `Amount` are original input features
- `Class` is the target variable:
  - `0` — normal transaction
  - `1` — fraudulent transaction

---

## Tools and Libraries

This project uses:

- Python
- Jupyter Notebook
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

---

# Analysis Steps

The project currently includes the following steps:

## 1. Data loading
- imported dataset into pandas DataFrame
- inspected the first rows

## 2. Dataset inspection
- checked number of rows and columns
- reviewed data types
- checked missing values
  
## 3. Target variable analysis
- explored fraud vs normal transaction distribution
- identified severe class imbalance

## 4. Transaction amount analysis
- analyzed distribution of transaction amounts
- identified right-skewed distribution and outliers

## 5. Further steps planned
- compare Amount for fraud vs non-fraud transactions
- analyze Time
- visualize feature relationships
- build a simple baseline model

# Key Findings
### 1. Dataset size:
- 284,807 transactions
- 31 features

### 2. Missing values:
- no missing values detected

### 3. Data types:
- all columns are numeric
- most features are float64
- `Class` is int64 and represents a binary target variable

### 4. Class imbalance:
- normal transactions: 284,315 (99.83%)
- fraudulent transactions: 492 (0.17%)
- This means the dataset is highly imbalanced, which is a critical issue for fraud detection tasks.
- Accuracy alone is not a reliable metric in such cases.

### 5. Amount distribution:
- transaction amounts are strongly right-skewed
- most transactions are concentrated at low values
- a small number of transactions have very large amounts
- the Amount feature contains outliers

# Why This Project Matters

## Fraud detection is a real-world analytics problem where data imbalance, anomaly detection, and business impact are all important.
This project helps practice:
- exploratory data analysis
- fraud-oriented analytical thinking
- interpreting distributions and imbalance
- preparing data for machine learning tasks

# Future Improvements

## Planned next steps:
- compare fraudulent and non-fraudulent transactions by amount
- explore the Time feature
- create additional visualizations
- evaluate baseline machine learning model
- analyze precision and recall instead of relying only on accuracy

<details>
 <summary> How to Run </summary>

1. Clone the repository
2. Create and activate a virtual environment
3. Install dependencies
4. Open the notebook

### Install dependencies:

```bash
pip install -r requirements.txt
```
### Run Jupyter Notebook:
```bash
jupyter notebook
```
or open the notebook directly in VSCode.
</details>

# Author

## Serhii Mamonov

### This project was created as part of practical training in data analysis, portfolio development, and preparation for junior data analyst / fraud analytics roles.
