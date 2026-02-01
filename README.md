
# 📦 Vendor Performance & Inventory Analytics (SQL + Python + Power BI)

## 📌 Project Overview
This project demonstrates a complete data pipeline and analytics workflow to analyze vendor performance, inventory movement, sales, and profitability.

The solution starts from raw CSV files, builds a structured inventory database in SQL using Python, performs data cleaning and feature engineering, conducts Exploratory Data Analysis (EDA), and finally delivers insights through an interactive Power BI dashboard.

---

## 🗂️ Data Source
5 Raw CSV files containing:
- Purchases
- Sales
- Purchase Prices
- Vendor Invoices (Freight)
- Product / Vendor details

---

## ⚙️ End-to-End Workflow

### Step 1 — Raw Data Ingestion into SQL Database
Python script reads all CSV files and loads them into a SQLite inventory database as separate tables.

### Step 2 — Creating Vendor Summary Table (SQL + Python)
Python script performs SQL joins and aggregations across tables to create a final vendor sales summary table.

### Step 3 — Data Cleaning & Feature Engineering
Derived metrics created:
- Gross Profit
- Profit Margin %
- Stock Turnover
- Sales to Purchase Ratio

### Step 4 — Exploratory Data Analysis (EDA)
EDA performed in Jupyter notebooks to analyze vendor contribution, sales vs profit, quantity vs revenue, and inventory efficiency.

### Step 5 — Power BI Dashboard
Power BI connects to the cleaned vendor_sales_summary table from SQL for visualization.

---

## 📊 Dashboard KPIs
| KPI | Value |
|---|---:|
| Total Sales | 200.94M |
| Total Purchase | 321.62M |
| Gross Profit | 130.00M |
| Profit Margin | 28.79% |
| Stock Turnover | 1.74 |
| Sales to Purchase Ratio | 2.55 |

---

## 🧠 Business Insights Delivered
- Identify high revenue but low profit vendors
- Detect low-performing vendors by sales and quantity
- Measure inventory efficiency
- Understand vendor profitability patterns

---

## 🛠️ Tech Stack
- Python (Pandas, SQLAlchemy, Logging)
- SQLite Database
- SQL (CTEs, Joins, Aggregations)
- Jupyter Notebook (EDA)
- Power BI

---

## 📁 Project Structure
data/                       → Raw CSV files
logs/                       → Execution logs
inventory.db                → SQLite database
GitIngest_db.py             → CSV → SQL ingestion
Git_get_vendor_summary.py   → Vendor summary creation
EDA_Notebooks.ipynb         → Exploratory analysis
Vendor_Performance.pbix     → Power BI dashboard

---

## ▶️ How to Run the Project

1. Place all CSV files inside /data folder
2. Run: python GitIngest_db.py
3. Run: python Git_get_vendor_summary.py
4. Open inventory.db or connect Power BI to it
5. Load vendor_sales_summary table into Power BI

---

## 👤 Author
Shashi Kumar Singh  
Data Analyst | Python | SQL | Power BI | Data Engineering


## Dashboard Snap 
<img width="617" height="333" alt="Image" src="https://github.com/user-attachments/assets/e78cd838-e91b-412f-b4ec-d3280436106e" />


## 🔗 Live Power BI Dashboard

Click here to view the interactive dashboard:  
https://app.powerbi.com/view?r=eyJrIjoiOGFkY2RkOGEtZWFmNy00NDI4LWE4OWEtZGY5YTBjNzEyYWZlIiwidCI6ImY4NTc3MjA3LWIwNWQtNDA0ZS04MmIzLTczMzcwMGNkYzE2ZCJ9
