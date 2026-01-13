# Zepto_SQL_Analysis using SQL (PostgreSQL)
SQL analysis of product pricing, discounts, and inventory data

## Project Overview
This project analyzes Zepto grocery product data using **SQL (PostgreSQL)** to derive insights related to pricing, discounts, stock availability, inventory weight, and revenue estimation.

The analysis follows a structured SQL workflow including table creation, data exploration, data cleaning, and business analysis.

---

## Dataset
This project uses a single dataset:

- `zepto_v2.csv`

The dataset contains product-level information such as:
- Product category
- Product name
- MRP
- Discount percentage
- Discounted selling price
- Available quantity
- Stock status
- Product weight

---

## Tools & Technologies
- PostgreSQL
- pgAdmin
- SQL
- CSV file

---

## Database Schema
The data is stored in a table named `zepto` with the following columns:

- `sku_id` (Primary Key)
- `category`
- `name`
- `mrp`
- `discountPercent`
- `availableQuantity`
- `discountedSellingPrice`
- `weightInGms`
- `outOfStock`
- `quantity`

---

## Analysis Performed

### Data Exploration
- Total number of records
- Sample data inspection
- Null value detection
- Distinct product categories
- In-stock vs out-of-stock analysis
- Identification of duplicate products

### Data Cleaning
- Removal of products with zero pricing
- Conversion of prices from paise to rupees

### Business Analysis
- Top discounted products
- High-MRP products that are out of stock
- Estimated revenue by category
- Premium products with low discounts
- Categories offering highest average discounts
- Price per gram analysis
- Product weight classification (Low, Medium, Bulk)
- Total inventory weight analysis

---

## How to Run the Project
1. Create the `zepto` table using the SQL script
2. Import `zepto_v2.csv` into PostgreSQL using pgAdmin
3. Execute the SQL queries in pgAdmin
4. Analyze the query results

> Note: CSV import is done using pgAdmin’s Import/Export feature.

---

## Repository Structure
├── zepto_analysis.sql
├── zepto_v2.csv
└── README.md

---

## Key Learnings
- Writing efficient SQL queries
- Performing data cleaning in SQL
- Extracting business insights from data
- Working with PostgreSQL and pgAdmin

Dataset sourced from Kaggle for educational and portfolio purposes.
