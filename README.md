# underwearWholesaling

# 🧱 Underwear Wholesaler – Data Engineering MVP

This project showcases a complete data engineering pipeline using PySpark and Databricks Community Edition, with a focus on building a **cloud-based star schema** and running SQL queries for business insights.

## 📦 Project Overview

We worked with a real-world style dataset for a fictional **underwear wholesaler**, involving customer transactions, product info, shipping methods, employees, and payments.

The pipeline follows the key stages of data engineering:
- Data ingestion
- Data cleaning and validation
- Schema modeling (star schema)
- Querying and insight generation

---

## 🗂️ Tools & Technologies

- 🧠 **Apache Spark (PySpark)**
- ☁️ **Databricks Community Edition**
- 🗃️ CSV files hosted on GitHub
- 🧹 DataFrames & SQL-based transformations
- 📊 Optional extensions to BI tools like Power BI or Streamlit

---

## 🧭 Project Structure

| Step | Description |
|------|-------------|
| 0. Context & Setup     | Project goals, imports, data source setup |
| 1. Data Loading        | Ingestion of 11 CSV files from GitHub via requests |
| 2. Data Cleaning       | Null analysis, dropping & filtering invalid records |
| 3. Schema Design       | Star schema structure: one fact table and six dimension tables |
| 4. Fact Table Creation | Combining and refining metrics from multiple sources |
| 5. Querying            | Using SQL to generate business insights from the warehouse |

---

## ⭐ Final Star Schema

- `fact_sales`
- `dim_customers`
- `dim_products`
- `dim_employees`
- `dim_shipping_methods`
- `dim_payment_methods`
- `dim_date`

Each dimension is normalized and linked via foreign keys to allow efficient querying and slicing across time, geography, and product categories.

---

## 📊 Example Insights

Queries were built to answer real business questions like:
- Which products sell the most?
- Who are our top customers?
- What is the average freight cost by shipping method?
- How does performance vary by employee or over time?

---

## 🚀 Future Improvements

- Add support for inventory or purchase order fact tables
- Export to Parquet / Delta format
- Build Streamlit dashboard or connect to Power BI
- Automate updates to warehouse via scheduled ETL
