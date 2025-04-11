# 🧾 Underwear Wholesale Analytics – End-to-End Data Engineering Project

Welcome to a complete data engineering and business analytics project built using **Apache Spark** and **Databricks**, simulating the real-world environment of a wholesale clothing distributor specializing in **intimate apparel**.

This project covers the full data pipeline lifecycle — from raw data ingestion to dimensional modeling, cleaning, and SQL-driven business insights — with the goal of delivering clear, actionable findings to support strategic decision-making across sales, operations, and customer success.

---

## 🎯 Objective

The goal of this project is to build a scalable data solution that enables deep analytical understanding of the company’s wholesale sales operation. This includes:

- Constructing a **Star Schema** model for optimized querying
- Cleaning and modeling raw transactional data into **dimension and fact tables**
- Leveraging **Spark SQL** to investigate core business performance
- Identifying **revenue drivers**, **customer behavior**, and **operational patterns**
- Delivering data-informed insights to support **growth strategies**, **account management**, and **market expansion**

---

## ❓ Key Business Questions Answered

This project explores and answers questions such as:

- What are the top revenue-generating **products**, **categories**, and **regions**?
- Which **customer segments**, **lead sources**, and **classes** are most profitable?
- What does the **employee performance landscape** look like in terms of orders, clients, and revenue?
- Where are the opportunities for growth based on **underpenetrated regions** and **high-value accounts**?
- What are the **shipping patterns**, and is there room for logistics optimization?
- What share of customers are **repeat clients** and what is their impact on revenue?
- What are the **trends over time**, and how is the business growing?

---

## 🧱 Data Pipeline & Star Schema Overview

This project uses an industry-standard **Star Schema** built around a central fact table `fact_sales` and the following dimensions:

| Table               | Description |
|--------------------|-------------|
| `dim_customers`     | Customer profile and segmentation attributes |
| `dim_products`      | Product metadata including category, gender, size |
| `dim_employees`     | Sales reps and employee codes |
| `dim_shipping_methods` | Delivery method per order |
| `dim_payment_methods`  | Available payment types |
| `dim_date`          | Calendar dimension extracted from orders and shipping dates |
| `dim_payments`      | Supplementary payment records (partial coverage) |

---

## 📁 Project Structure

The project is divided into the following main sections:

### 0 – 🧰 Project Initialization  
- 💻 Environment Setup  
- 🌐 GitHub API access to retrieve CSVs

### 1 – ⚙️ Data Loading & Initial Fixes  
- 💾 File download and load into Spark  
- ⚠️ Encoding fixes for key datasets  

### 2 – 🧹 Initial Data Quality Checks  
- 🔍 Nulls, Duplicates & Distinct Counts  
- 🧼 Data cleaning decisions based on context

### 3 – 🧱 Building the Enriched Fact Table  
- 📦 Joining orders and line-item details  
- 👥 Enriching with customers and employees  
- 🚚 Adding product and shipping metadata  
- 💳 Integrating payments and payment methods  

### 4 – ⭐ Building the Star Schema  
- 🧑‍💼 Creating clean dimension tables  
- 🧾 Final fact table created and validated  

### 5 – 📊 Business Questions & Strategic Insights  
- Sales coverage vs. paid order comparison  
- Revenue breakdown by product, gender, region  
- Customer loyalty, account profiling, and AOV  
- Employee performance metrics  
- Time series insights and shipping analysis  

### 6 – ✅ Final Considerations  
- Observations on data quality issues  
- Key takeaways on customer behavior and product mix  
- Recommendations for future data collection and optimization

---

## ⚙️ Tools & Technologies

This project was developed using:

- **Apache Spark (PySpark)** on **Databricks Community Edition**
- **Spark SQL** for querying the star schema  
- **Python** for data preprocessing and logic
- **GitHub** for version control and public data hosting
- **Markdown** for documentation and insights presentation

---

## 📌 Final Notes

Despite partial gaps in payment and shipping data, the project demonstrates how to build a reliable analytical pipeline and surface high-value insights even when working with real-world data limitations. This includes:
- Creating a clean and scalable data model
- Delivering meaningful KPIs for decision-makers
- Providing structure for future enhancements like benchmarking, time series forecasting, or dashboard integration

---

---

## ▶️ How to Run This Project

This project was developed on **Databricks Community Edition** using **PySpark**. To replicate or run it yourself, follow the steps below:

### 1. Clone the Repository

Download or clone this repository to access the raw CSV files and notebook structure.

```bash
git clone https://github.com/Barbosa6Andre/underwearWholesaling.git
