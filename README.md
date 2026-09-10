# 🛒 Zepto E-commerce Inventory Data Analysis

**SQL + Power BI Portfolio Project**

A complete end-to-end data analysis project on Zepto’s product inventory dataset. This project demonstrates real-world data analyst workflows — from raw data exploration and cleaning to generating actionable business insights using SQL, with visualization support in Power BI.

---

## 📌 Project Overview

Zepto is one of India’s leading quick-commerce platforms. This project analyzes a scraped product inventory dataset to uncover insights related to:

- Pricing & discount strategies
- Stock availability & inventory health
- Category-level performance
- Revenue potential
- Product value (price per gram)

The goal is to simulate how a data analyst would work with messy real-world e-commerce inventory data.

---

## 🛠️ Tools & Technologies

| Category          | Tools Used          |
|-------------------|---------------------|
| Database          | PostgreSQL / MySQL  |
| Query Language    | SQL                 |
| Visualization     | Power BI            |
| Dataset           | Zepto Product Inventory (CSV) |

---

## 📁 Dataset Overview

**File:** `Zepto_v2.csv`  
**Source:** Scraped from Zepto’s public product listings (available on Kaggle)

### Columns

| Column                  | Description                                      |
|-------------------------|--------------------------------------------------|
| `sku_id`                | Unique product identifier (synthetic primary key)|
| `category`              | Product category (e.g., Fruits & Vegetables)     |
| `name`                  | Product name                                     |
| `mrp`                   | Maximum Retail Price (originally in paise)       |
| `discountPercent`       | Discount percentage                              |
| `availableQuantity`     | Current available stock                          |
| `discountedSellingPrice`| Selling price after discount (originally in paise)|
| `weightInGms`           | Product weight in grams                          |
| `outOfStock`            | Boolean flag for stock status                    |
| `quantity`              | Quantity per unit                                |

---

## 🔍 Project Structure


---

## 🧹 Data Cleaning Steps

1. Checked for null values across all columns
2. Identified and removed products with `mrp = 0`
3. Converted prices from **paise to rupees** (`mrp` and `discountedSellingPrice`)
4. Explored duplicate product names and stock distribution

---

## 📊 Key Business Analyses Performed

| #  | Analysis Question                                                                 | Insight Area              |
|----|------------------------------------------------------------------------------------|---------------------------|
| 1  | Top 10 best-value products based on discount percentage                            | Pricing Strategy          |
| 2  | High MRP products that are currently out of stock                                  | Inventory Risk            |
| 3  | Estimated revenue by category                                                      | Revenue Potential         |
| 4  | Products with MRP > ₹500 and discount < 10%                                        | Pricing Opportunities     |
| 5  | Top 5 categories with highest average discount percentage                          | Category Performance      |
| 6  | Price per gram for products ≥ 100g (best value products)                           | Value for Money           |
| 7  | Product weight segmentation (Low / Medium / Bulk)                                  | Inventory Classification  |
| 8  | Total inventory weight per category                                                | Supply Chain Insights     |

---

## 🚀 How to Run the Project

### 1. Database Setup
```sql
-- Create table and load data
-- Run the entire script in zepto_analysis.sql


2. Recommended Tools
•  PostgreSQL + pgAdmin / DBeaver
•  MySQL Workbench
•  Power BI for dashboard creation
3. Steps
1.  Create a new database
2.  Run the table creation script from zepto_analysis.sql
3.  Import Zepto_v2.csv
4.  Execute the exploration, cleaning, and analysis queries sequentially
5.  Connect the cleaned data to Power BI for visualization (optional)

