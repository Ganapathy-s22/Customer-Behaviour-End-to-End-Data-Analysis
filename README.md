# 📊 Customer Behaviour End-to-End Data Analytics Project

## 🎯 Business Objective
The primary goal of this project is to analyze customer purchasing patterns, subscription distributions, and revenue pipelines to extract actionable business insights. By profiling customer demographics (Age Groups, Gender) and behavioral metrics (Shipping choices, Review Ratings), this analysis provides corporate stakeholders with strategies to optimize product stock and marketing campaign targeting.

---

## 🛠️ Data Analytics Pipeline & Tech Stack

### 🟦 Phase 1: Data Wrangling & Cleaning (Python - Pandas)
* **Tool Used:** Jupyter Notebook (Python 3)
* **Operations Executed:**
  * Imported the raw structural messy dataset and inspected data types.
  * Handled missing/null values safely using business-context boundaries to prevent data distortion.
  * Dropped structural duplicate rows (`drop_duplicates()`) and isolated extreme outliers.
  * Categorized continuous numerical data into discrete bins (e.g., Transforming raw ages into `Young Adult`, `Middle-aged`, `Adult`, and `Senior`).
  * Exported the high-quality unified asset as `cleaned_customer_data.csv`.

### 🗄️ Phase 2: Structural Insights & Database Queries (SQL - PostgreSQL)
* **Tool Used:** pgAdmin 4 / PostgreSQL Server
* **Operations Executed:**
  * Imported the `cleaned_customer_data.csv` as a structural relational table.
  * Wrote optimized analytical queries using advanced aggregation and grouping logic (`GROUP BY`).
  * **Key Business Queries Resolved:**
    * *Q1:* Total revenue generated split by Male vs. Female customer segments.
    * *Q2:* Identification of high-spending customers utilizing active discounts.
    * *Q3:* Ranking top 5 performing product categories by average review ratings.

### 📊 Phase 3: Interactive Visual Modeling (Power BI)
* **Tool Used:** Power BI Desktop
* **Operations Executed:**
  * Established a live semantic data link to the PostgreSQL server engine.
  * Designed an advanced corporate executive layout with a dedicated **Slicers Filtering Panel** (Subscription, Gender, Category, Shipping Type).
  * Built functional custom **DAX Measures** for dynamic KPI rendering (Total Customers, Avg Purchase, Avg Rating).

---

## 📈 Dashboard Layout & Visual Metrics Archetype

The final interactive reporting structure delivers multi-layered business metrics at a glance:

* **Executive KPI Panel:** Displays $3.9\text{K}$ active customers, an average purchase ticket size of $\$59.76$, and a solid customer satisfaction anchor at $3.75$ average rating.
* **Subscription Matrix:** A clean Donut Chart showing that while $73\%$ are standard users, a core premium base of $27\%$ drive subscription loyalty.
* **Category Performance:** Vertical Bar charts highlighting **Clothing** as the absolute dominant driver in both transaction count ($1737$ sales) and total revenue ($\$104\text{K}$), closely followed by Accessories.
* **Age Demographics Breakdown:** Horizontal comparative charts mapping **Revenue vs. Sales Volume** across generations, proving that **Young Adults** represent the highest lifetime value (LTV) cohort.

---

## 📁 Repository Structure
```text
├── Business Problem Document.pdf       # Project requirement guide
├── raw_customer_behaviour_file         # Raw customer dataset (Input)
├── cleaned_customer_data.csv           # Processed clean data after Pandas pipeline
├── data_cleaning.ipynb                 # Jupyter Notebook with Python cleaning steps
├── customer_behavior_sql_queries.sql   # PostgreSQL database analysis queries
├── first_project_on_powerbi.pbix       # Final interactive Power BI working model
└── first_project_on_powerbi.pdf        # Static PDF export of the executive dashboard
└── README.md                           # Documentation and business insights profile
