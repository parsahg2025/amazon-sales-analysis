# Amazon Sales Analysis: Trend Discovery & Anomaly Detection

## 📌 Project Overview
This project performs an in-depth exploratory and statistical analysis of 50,000 Amazon sales transactions. The goal is to uncover hidden consumer shopping patterns using **Frequent Itemset Mining** and to identify high-value or fraudulent transactions through **Unsupervised Anomaly Detection**. 

By integrating course-standard algorithms with advanced statistical validation (ANOVA and Chi-squared tests), this project provides a data-driven framework for understanding regional market dynamics and operational outliers.

## 🛠️ Tech Stack & Methodologies
- **Data Manipulation**: Python (Pandas, NumPy)
- **Machine Learning**: Scikit-Learn (Isolation Forest)
- **Association Rule Mining**: MLxtend (Apriori Algorithm)
- **Statistical Analysis**: SciPy (ANOVA, Chi-squared Test of Independence)
- **Visualization**: Matplotlib, Seaborn

## 🔍 Key Analytical Components

### 1. Anomaly Detection (Course Topic)
Utilizing the **Isolation Forest** algorithm, we isolated outliers that represent transactions with unusual price-to-quantity ratios or extreme revenue values that deviate from standard regional behavior.

### 2. Frequent Itemset Mining (Course Topic)
Using the **Apriori** algorithm, we analyzed category co-occurrences. This identifies which product categories are most likely to be purchased together, providing insights for cross-selling strategies.

### 3. Statistical Significance Testing (Beyond-Course)
To ensure findings are robust, we applied:
- **ANOVA**: Testing if mean revenue across product categories varies significantly.
- **Chi-squared Test**: Determining the independence between geographical regions and payment methods.

## 📊 Dataset Description
The analysis is based on the [Amazon Sales Dataset](https://www.kaggle.com/datasets/aliiihussain/amazon-sales-dataset). 
- **Size**: 50,000 rows, 13 features.
- **Key Features**: `order_id`, `product_category`, `total_revenue`, `customer_region`.

## 📂 Repository Structure
```text
├── notebooks/          # Jupyter notebooks with step-by-step analysis
│   └── 01_EDA_Statistical_Tests.ipynb
├── README.md           # Project executive summary
└── .gitignore          # Prevents uploading unnecessary local files
