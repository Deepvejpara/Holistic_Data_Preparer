# 🏦 Customer Credit Risk Analysis & Data Preprocessing Project

## 📌 Objective

This project aims to demonstrate a complete **Data Preprocessing & Feature Engineering pipeline** for a real-world fintech problem — predicting whether a customer will **default on a loan**.

The goal is to transform raw, messy data into a **clean, ML-ready dataset**.

---

## 🧠 Problem Statement

You are working as a **Junior Data Scientist** at a fintech company.
The dataset is collected from multiple sources (CSV, JSON, SQL, API).

Your task:

* Perform **data cleaning**
* Handle **missing values & outliers**
* Apply **feature engineering**
* Prepare data for a **Machine Learning model**

🎯 Target Variable:

* `default_flag` → (0 = No Default, 1 = Default)

---

## 📊 Dataset Overview

### 🔑 Features

| Column            | Description                           |
| ----------------- | ------------------------------------- |
| customer_id       | Unique customer ID                    |
| age               | Customer age                          |
| gender            | Male / Female / Other                 |
| region            | North / South / East / West           |
| education_level   | Primary → Post-Graduate               |
| employment_type   | Salaried / Self-Employed / Unemployed |
| annual_income     | Annual income (₹)                     |
| loan_amount       | Loan requested (₹)                    |
| loan_purpose      | Home / Car / Education / Business     |
| credit_score      | Score (300–850)                       |
| repayment_history | Missed payments                       |
| transaction_count | Transactions (last 6 months)          |
| spending_ratio    | Spending-to-income ratio              |
| join_date         | Account creation date                 |
| default_flag      | Target variable                       |

---

## ⚙️ Data Preprocessing Steps

### 🧹 1. Data Cleaning

* Checked null values using `.info()` and `.describe()`
* Generated data quality insights

---

### ❗ 2. Missing Value Handling

* **Numerical:** Mean / Median Imputation
* **Categorical:** Most Frequent Imputation
* **Advanced:**

  * KNN Imputer
  * MICE
  * Missing Indicator

---

### 📉 3. Outlier Detection

* Z-score Method
* IQR Method
* Percentile Method
* Winsorization

---

### 🔄 4. Feature Engineering

#### 🧮 New Features

* `debt_to_income` = loan_amount / annual_income
* `avg_transaction`
* `spending_ratio`

#### 🔁 Transformations

* Log Transform
* Square Root
* Box-Cox / Yeo-Johnson

---

### 🔤 5. Encoding

* **Ordinal Encoding** → education_level
* **Label Encoding** → gender
* **One-Hot Encoding** → region, loan_purpose

---

### 📊 6. Feature Scaling

* Standardization (Z-score)
* Min-Max Scaling
* Robust Scaling

---

### 🔢 7. Binning / Discretization

* Income grouping
* Credit score segmentation
* Quantile binning
* K-Means binning

---

### 📅 8. Date Feature Extraction

From `join_date`:

* Year
* Month
* Day
* Weekday

---

## 🚀 Final Output

* Cleaned dataset
* Transformed features
* No missing values
* Outliers handled
* Fully ready for ML model training

---

## 🛠️ Tech Stack

* Python 🐍
* Pandas
* NumPy
* Scikit-learn

---

## 📂 Project Structure

```
├── data/
│   └── loan_dataset.csv
├── notebooks/
│   └── preprocessing.ipynb
├── README.md
```

---

## 📈 Expected Outcome

By completing this project, you will:

* Understand real-world **data preprocessing workflows**
* Learn **advanced feature engineering**
* Prepare datasets for **machine learning models**
* Build a strong **portfolio project**

---

## 💡 Future Improvements

* Add ML model (Logistic Regression / Random Forest)
* Hyperparameter tuning
* Model evaluation (ROC-AUC, Precision, Recall)

---

## 👨‍💻 Author

**Deep**
Aspiring Data Scientist 🚀

---

⭐ If you found this useful, consider giving it a star!
