# DE Daily Practice 📚

A daily log of my Data Engineering learning journey — SQL, Python, PySpark, and more.

---

## 📅 Progress Tracker

| Day | Topic | Status |
|-----|-------|--------|
| Day 1 | Advanced SQL | ✅ Done |
| Day 2 | Python ETL | ✅ Done |
| Day 3 | Data Modelling | ✅ Done |
| Day 4 | PySpark Basics | ✅ Done |
| Day 5 | PySpark Advanced + SparkSQL | ✅ Done |
| Day 6 | Delta Lake + Medallion Architecture | ✅ Done |
| Day 7 | Databricks Workflows | ✅ Done |
| Day 8 | Azure ADLS Gen2 | 🔄 In Progress |
| Day 9 | Azure Data Factory Part 1 | ⬜ Upcoming |
| Day 10 | Azure Data Factory Part 2 | ⬜ Upcoming |
| Day 11 | Azure Synapse Analytics | ⬜ Upcoming |
| Day 12 | Power BI | ⬜ Upcoming |
| Day 13 | Capstone Project | ⬜ Upcoming |
| Day 14 | Interview Prep | ⬜ Upcoming |

---

## 📂 Folder Structure

de-daily-practice/
├── sql-practice/
│   └── day1_sql.sql        # Window functions, CTEs, Joins, Optimisation, PIVOT
├── day2_python/
│   └── etl.py              # Python ETL pipeline with logging and error handling
├── day3_modelling/
│   └── day3_schema.sql     # Star schema design for e-commerce
└── README.md

---

## 🛠️ Stack

![SQL](https://img.shields.io/badge/SQL-PostgreSQL-blue)
![Python](https://img.shields.io/badge/Python-3.12-yellow)
![PySpark](https://img.shields.io/badge/PySpark-Databricks-red)
![Delta Lake](https://img.shields.io/badge/Delta-Lake-green)
![Azure](https://img.shields.io/badge/Azure-ADLS%20%7C%20ADF%20%7C%20Synapse-0078D4)
![Power BI](https://img.shields.io/badge/Power-BI-F2C811)

---

## 📝 Day 1 — Advanced SQL

**Topics covered:**
- Window Functions — ROW_NUMBER, RANK, DENSE_RANK, LAG, LEAD, NTILE
- CTEs — basic and chained
- Complex Joins — self join, anti join, cross join
- Subqueries vs CTEs
- Query Optimisation — indexes, EXPLAIN, avoiding SELECT *
- PIVOT / UNPIVOT

**Dataset:** `employees` table — 10 employees across Engineering, Marketing, HR

**Key learnings:**
- DENSE_RANK is preferred over RANK for top-N queries to avoid gaps
- CTEs improve readability and allow reuse of logic
- Anti join = LEFT JOIN + WHERE right.id IS NULL
- Always filter with WHERE before HAVING for performance

---

## 📝 Day 2 — Python ETL

**Topics covered:**
- Reading CSV with Pandas
- Data cleaning — nulls, duplicates, type casting
- Column transformations with lambda functions
- Reusable functions with docstrings
- Logging with Python logging module
- Error handling with try/except
- Writing output as Parquet

**Key learnings:**
- Always use logging over print in production scripts
- Wrap pipelines in try/except to handle failures gracefully
- Parquet is preferred over CSV for analytical workloads

---

## 📝 Day 3 — Data Modelling

**Topics covered:**
- ETL vs ELT
- Batch vs Streaming
- Full load vs Incremental load
- Star schema vs Snowflake schema
- SCD Type 1, 2, 3
- Fact tables vs Dimension tables

**Key learnings:**
- Star schema is denormalised — faster queries, preferred for BI
- SCD Type 2 adds a new row to preserve history
- DimDate is always generated, not sourced

---

## 📝 Day 4 — PySpark Basics

**Topics covered:**
- SparkSession
- Creating DataFrames
- select, filter, withColumn, groupBy, agg, orderBy
- Joins in PySpark
- Writing Delta tables with saveAsTable

---

## 📝 Day 5 — PySpark Advanced + SparkSQL

**Topics covered:**
- Transformations vs Actions
- SparkSQL with createOrReplaceTempView
- Window functions in PySpark
- UDFs — when to use and avoid
- Broadcast joins
- Null handling — dropna, fillna, coalesce

---

## 📝 Day 6 — Delta Lake + Medallion Architecture

**Topics covered:**
- Delta Lake vs Parquet
- Bronze → Silver → Gold pipeline
- Time travel — VERSION AS OF
- MERGE / UPSERT
- OPTIMIZE
- DESCRIBE HISTORY

---

## 📝 Day 7 — Databricks Workflows

**Topics covered:**
- Created 3 separate notebooks (bronze, silver, gold)
- Built medallion_pipeline workflow with 3 sequential tasks
- Pipeline ran successfully in 42 seconds

---

## 👩‍💻 About

IT Graduate from UPM Malaysia, actively building Data Engineering skills.

Target: Junior Data Engineer role in Malaysia
