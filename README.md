# 🚀 What Drives Online Purchases?
## A Data Mining Study of Pricing Signals and Social Proof in Amazon Sales

🎥 **Project Video (2 min):** https://youtu.be/85tgdwctryA  
👉 **Start here:** [`main_notebook.ipynb`](main_notebook.ipynb)

---

## 🧭 Where Should You Start?

If you're new to this project, follow this simple path:

1️⃣ Watch the short project video  
2️⃣ Open 👉 **`main_notebook.ipynb`**  
3️⃣ Use this README to understand the context  

📌 The notebook is the **main deliverable**.  
Everything here is designed to help you understand it better — not replace it.

---

## 📌 Project Overview

**❓ Do higher discounts and more reviews actually lead to more sales — or are these just common myth in e-commerce? ❓**

This project takes a data-driven approach to evaluate whether **pricing signals** (discounts and ratings) and **social proof** (review count) are meaningfully associated with purchasing behavior. Using a dataset of 50,000 Amazon transactions, the analysis applies data mining techniques to test whether these widely used signals truly influence how much customers buy.

This project tests that assumption using data.

Using a dataset of **50,000 Amazon transactions**, the analysis evaluates whether:

- pricing signals (**discounts and ratings**)  
- social proof (**review count**)  

are meaningfully associated with **quantity sold**.

⚠️ Instead of assuming these assumptions work, this project **measures their actual impact**.

👉 The full analytical story, including visuals and interpretations, is presented in:  
**`main_notebook.ipynb`**

---

## ❓ The Questions We’re Trying to Answer

This project focuses on two tightly connected questions:

### 🔹 RQ1 — **Pricing Signals: Do Discounts & Ratings Drive Sales?**

👉 Explored using **association rule mining**

---

### 🔹 RQ2 — **Social Proof: Do products with more reviews sell more?**

👉 Explored using **cross-tabulation and probability analysis**

---

📌 These questions are fully explored, visualized, and interpreted in:  
👉 **`main_notebook.ipynb`**

---

## 📊 Data

- **Dataset:** Amazon Sales Dataset (Kaggle)  
- **Size:** 50,000 transactions  
- **Location:** `data/amazon_sales_dataset.csv`

The notebook also includes code to download the dataset directly.

---

### 🧹 Preprocessing (High-Level)

To support pattern analysis:

- Data was validated (missing values, duplicates, invalid ratings)
- Numerical variables were converted into categories:

| Variable | Categories |
|---|---|
| Discount | Low / Mid / High |
| Rating | Poor / Average / High |
| Quantity | Single / Multi / Bulk |
| Reviews | Niche / Steady / Popular |

📌 Full preprocessing details are available in:  
`checkpoints/preprocessing.ipynb`  

📌 Only the **clean, final version** is used in:  
👉 **`main_notebook.ipynb`**

---

## 🧠 Analysis Approach

### 🔹 RQ1 — Association Rule Mining

Used the **Apriori algorithm** to find patterns like:

Condition(s) → Outcome

Evaluated using:
- Support
- Confidence
- Lift (key metric)

📌 Interpretation of these rules is provided in:  
👉 **`main_notebook.ipynb`**

---

### 🔹 RQ2 — Cross-Tabulation

Analyzed:

P(Bulk Purchase | High Reviews)

to understand whether review count affects purchasing behavior.

📌 Category-level comparisons and insights are in:  
👉 **`main_notebook.ipynb`**

---

## 📈 Key Findings

### 🔹 Pricing Signals
- Higher discounts ≠ significantly higher sales  
- Higher ratings ≠ significantly higher sales  
- Most relationships are **weak (lift ≈ 1)**  

---

### 🔹 Social Proof
- Products with more reviews do **not** strongly sell more  
- Bulk purchase probability remains stable (~39%–42%)  

---

## 🎯 Main Takeaway

> **Simple marketplace signals do not strongly explain purchasing behavior.**

This challenges a common assumption in e-commerce.

📌 Full interpretation and discussion are in:  
👉 **`main_notebook.ipynb`**

---

## 🤔 Why This Matters

Businesses often rely on:

- discounts  
- ratings  
- review counts  

But this analysis suggests:

➡️ These signals alone are not enough  

Customer decisions likely depend on:

- pricing strategy  
- brand reputation  
- delivery speed  
- return policy  
- customer preferences  

---

## ▶️ How to Reproduce

This project was built in **Google Colab** using:

`Python 3.12.13`

The full environment is provided in:

`requirements.txt`

### Step 1: Clone the Repository

```bash
git clone <[your-repository-url](https://github.com/parsahg2025/amazon-sales-analysis)>
cd <amazon-sales-analysis>
```

### Step 2: Install Requirements

```bash
pip install -r requirements.txt
```

### Step 3: Open the Main Notebook

Open:

`main_notebook.ipynb`

This is the curated final notebook and should be run first.

### Step 4: Run the Notebook

Run all cells in order.

The dataset is included locally in:

`data/amazon_sales_dataset.csv`

The notebook may also download the dataset from Kaggle if needed.

---



⚙️ Key Dependencies

Python 3.12.13

pandas 2.2.2

numpy 2.0.2

matplotlib 3.10.0

seaborn 0.13.2

scipy 1.16.3

mlxtend 0.23.4


📌 Full list in: requirements.txt

