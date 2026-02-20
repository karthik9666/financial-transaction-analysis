📊 Financial Transaction Fraud Analysis
📌 Project Overview

This project analyzes financial transaction data to understand customer spending behavior, identify abnormal transaction patterns, and explore fraud-related indicators.

The goal is to perform structured data cleaning, feature engineering, exploratory data analysis (EDA), and statistical validation before applying fraud detection logic.

🎯 Objective

Clean and preprocess multi-source financial datasets

Merge user, card, and transaction data

Detect anomalies using statistical methods

Analyze spending patterns across transaction types

Study relationships between income, debt, and credit behavior

🎯 Objective

Clean and preprocess multi-source financial datasets

Merge user, card, and transaction data

Detect anomalies using statistical methods

Analyze spending patterns across transaction types

Study relationships between income, debt, and credit behavior


📂 Dataset

Source: Kaggle – Financial Transactions Dataset

The project uses the following datasets:

users_data.csv – Customer demographic and financial information

cards_data.csv – Card-level details (credit limit, brand, chip status, etc.)

transactions_data.csv – Transaction records

mcc_codes.json – Merchant category descriptions

train_fraud_labels.json – Fraud labels for transactions


🛠 Tech Stack

Python

Pandas

NumPy

Jupyter Notebook

Git & GitHub


🔄 Data Processing Workflow
1️⃣ Data Cleaning

Converted monetary columns from string to numeric format

Converted date columns to datetime format

Handled missing values logically (e.g., ONLINE transactions)

Removed duplicate records

2️⃣ Feature Engineering

Created Time_left_until_retirement feature

Calculated account active duration

Derived transaction-level statistical thresholds

3️⃣ Data Integration

Merged users, cards, and transactions using multi-column joins

Integrated fraud labels with transaction data

Mapped MCC codes to merchant descriptions

4️⃣ Exploratory Data Analysis

Transaction value distribution analysis

Percentile-based spending analysis

Outlier detection using IQR method

Credit limit and income distribution study

Gender-based financial comparison

Correlation analysis between income and debt


📈 Key Insights

Income-related variables show strong positive correlation.

Higher credit limits are associated with specific card brands.

Transaction type impacts average transaction value.

Outlier detection highlights extreme spending behavior.

Missing merchant state values were logically linked to online transactions.


| Percentile    | Transaction Value (USD) |
| ------------- | ----------------------- |
| 25th          | Below $8.93             |
| 50th (Median) | Below $28.99            |
| 75th          | Below $63.71            |
| 95th          | Below $167.50           |
| 99th          | Below $389.45           |


🚀 Future Improvements

Implement machine learning fraud classification model

Develop Power BI dashboard for real-time financial reporting

Add time-series anomaly detection

Create modular Python pipeline (src/ structure)



📌 Conclusion

This project demonstrates end-to-end financial data preprocessing, validation, integration, and analytical exploration aligned with real-world fraud analytics workflows. It reflects practical data cleaning strategies and analytical reasoning required in financial data roles.