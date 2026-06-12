# 🔍 SQL Exploratory Data Analysis Project

A structured, end-to-end exploratory data analysis (EDA) project using **T-SQL** against a data warehouse database. The project moves systematically from raw database exploration through to business-ready customer and product reports, demonstrating a range of analytical techniques used in real-world financial and commercial analysis.

---

## 📌 Project Overview

This project applies SQL-based analytics to a relational data warehouse, uncovering trends, performance patterns, and customer/product insights. It is structured as a progressive series of scripts — each building on the last — reflecting how an analyst would approach a new dataset in a professional setting.

**Tools & Technologies**
- T-SQL (Microsoft SQL Server)
- SQL Server Management Studio (SSMS)
- Data Warehouse schema (fact & dimension tables)

---

## 📁 Project Structure

```
SQL-Exploratory-Data-Analysis-Project/
│
├── datasets/               # Source data and database backup
├── scripts/                # All T-SQL analytical scripts (numbered sequentially)
├── docs/                   # Supporting documentation
├── LICENSE
└── README.md
```

---

## 🗂️ Scripts Breakdown

The scripts are numbered to reflect the natural analytical workflow:

| # | Script | Description |
|---|--------|-------------|
| 00 | `00_init_database.sql` | Initialises the database and sets up the environment |
| 01 | `01_database_exploration.sql` | Explores tables, schemas, row counts and data types |
| 02 | `02_dimensions_exploration.sql` | Profiles dimension tables — customers, products, geography |
| 03 | `03_date_range_exploration.sql` | Identifies the date range and time coverage of the data |
| 04 | `04_measures_exploration.sql` | Reviews key numeric measures — sales, quantity, cost |
| 05 | `05_magnitude_analysis.sql` | Analyses scale and distribution of key metrics |
| 06 | `06_ranking_analysis.sql` | Ranks products, customers and categories by performance |
| 07 | `07_change_over_time_analysis.sql` | Tracks trends and YoY / MoM changes across time periods |
| 08 | `08_cumulative_analysis.sql` | Running totals and cumulative revenue/growth metrics |
| 09 | `09_performance_analysis.sql` | Benchmarks actual vs average/expected performance |
| 10 | `10_data_segmentation.sql` | Segments customers and products into meaningful groups |
| 11 | `11_part_to_whole_analysis.sql` | Calculates category contribution as % of total |
| 12 | `12_report_customers.sql` | Final consolidated customer report with KPIs |
| 13 | `13_report_products.sql` | Final consolidated product report with KPIs |

---

## 💡 Key Analytical Techniques Demonstrated

- **Exploratory profiling** — row counts, null checks, distinct value analysis, date boundary detection
- **Trend analysis** — month-over-month and year-over-year revenue changes using window functions
- **Cumulative analytics** — running totals with `SUM() OVER (ORDER BY date)`
- **Ranking** — `RANK()`, `DENSE_RANK()`, `ROW_NUMBER()` to surface top/bottom performers
- **Segmentation** — CASE-based bucketing of customers by spend tier and purchase frequency
- **Part-to-whole** — percentage contribution queries to understand category and product mix
- **Performance benchmarking** — comparing individual records against averages using window aggregates
- **Report generation** — multi-metric summary reports combining joins, aggregations and derived columns

---

## 📊 Sample Insight Areas

- Which products and categories drive the most revenue?
- How has sales performance trended over time?
- Which customer segments contribute the most value?
- Where are the largest gaps between expected and actual performance?
- What does cumulative growth look like across the full date range?

---

## 🚀 How to Run

1. Restore the database from the `.bak` file in the `/datasets` folder using SQL Server Management Studio (SSMS)
2. Open scripts in numerical order starting from `00_init_database.sql`
3. Execute each script against the restored database
4. Scripts `12` and `13` produce the final customer and product reports

**Requirements:** Microsoft SQL Server (2019+) or SQL Server Express · SSMS or Azure Data Studio

---

## 👤 Author

**Kelechi Madubuko** — Financial & Data Analyst  
[LinkedIn](https://www.linkedin.com/in/kelechimadubuko/) · [GitHub](https://github.com/Khaylechy)
