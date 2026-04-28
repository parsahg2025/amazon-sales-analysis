## 📊 Dataset Description

This project uses the **Amazon Sales Dataset** available on Kaggle:

🔗 https://www.kaggle.com/datasets/aliiihussain/amazon-sales-dataset  

---

### 🧾 Overview

The dataset contains synthetic but realistic **Amazon-style e-commerce transaction data** designed for:

- data analysis  
- visualization  
- machine learning applications  

It captures key aspects of online retail behavior, including pricing, discounts, ratings, and customer interactions.

The dataset reflects **time-series sales patterns** and includes multiple product categories and regions, making it suitable for studying purchasing behavior and demand patterns.

---

### 📊 Key Features

The dataset includes:

- 📈 Time-based order data (sales over time)  
- 🛍️ Multiple product categories  
- 💸 Pricing and discount information  
- 🌍 Customer regional data  
- ⭐ Ratings and review metrics  
- 📦 Revenue-related variables  

These features allow for analysis of how different factors influence purchasing behavior. :contentReference[oaicite:1]{index=1}

---

### 🧩 Columns Included

The dataset contains the following main variables:

| Column | Description |
|---|---|
| `order_id` | Unique identifier for each order |
| `order_date` | Date of the transaction |
| `product_id` | Unique product identifier |
| `product_category` | Category of the product |
| `price` | Original product price |
| `discount_percent` | Discount applied (%) |
| `discounted_price` | Final price after discount |
| `quantity_sold` | Number of units purchased |
| `total_revenue` | Total revenue from the order |
| `customer_region` | Geographic region of the customer |
| `payment_method` | Payment type used |
| `rating` | Product rating |
| `review_count` | Number of customer reviews |

These variables support analysis of both **pricing strategies** and **customer behavior patterns**.

---

### ⚠️ Important Notes

- The dataset is **synthetically generated**, meaning it is not directly scraped from Amazon but designed to reflect realistic patterns. 
- It is suitable for **learning, experimentation, and modeling**, but conclusions should not be interpreted as real-world business evidence.  

---

### 📌 How This Project Uses the Dataset

From the full dataset, this project focuses on:

- `discount_percent` → pricing signal  
- `rating` → product quality signal  
- `review_count` → social proof signal  
- `quantity_sold` → purchasing behavior  

These variables are used to investigate whether common e-commerce signals are strongly associated with sales outcomes.

---

### 📜 License

The dataset is released under **CC0 (Public Domain)**, meaning it is free to use without restrictions.
