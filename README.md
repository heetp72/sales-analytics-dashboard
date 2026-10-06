# Sales Analytics Dashboard

A SQL-and-Power-BI sales analytics project focused on understanding revenue, profitability, product performance, and loss drivers in a retail sales dataset.

## Dashboard Preview

![Dashboard Preview](dashboard/dashboard-screenshot.png)

---

## Project Overview

This project analyzes a retail Superstore dataset to answer key business questions such as:

- Which product categories generate the most sales and profit?
- Which sub-categories and products are driving losses?
- How do sales trends change over time?
- Which regions or product mix decisions most impact profitability?

The workflow combines:

- SQL-based data import and cleaning
- Exploratory analysis and aggregation queries
- Analytical views for reporting
- Business-focused metrics for decision support
- Power BI dashboard design and presentation

---

## Business Context

The dataset contains transactional sales records with details across products, customers, geography, and order metrics. The goal is to identify where performance is strong, where margin is being eroded, and which actions can improve profitability.

Key business areas analyzed:

- Category performance
- Sub-category loss analysis
- Top profitable vs. loss-making products
- Monthly sales trends
- Profit margin by category

---

## Dataset

This project uses a Superstore-style retail sales dataset that includes:

- Sales
- Profit
- Quantity
- Discount
- Order date
- Product category and sub-category
- Product name and ID
- Region, state, city, and country
- Customer and order identifiers

The dataset is prepared and transformed using MySQL before being modeled for dashboard reporting.

---

## Tools and Technologies

- MySQL
- SQL
- Power BI
- DAX
- Data modeling
- Business reporting

---

## SQL Workflow

The repository is organized into a staged SQL process:

1. 01_data_import_cleaning.sql
   - Creates the database and loads raw sales data
   - Converts and validates data types
   - Cleans columns and checks null values

2. 02_exploratory_analysis.sql
   - Reviews category revenue
   - Identifies loss-making sub-categories
   - Examines monthly sales trend
   - Finds top profitable and loss-making products

3. 03_analytical_views.sql
   - Builds reusable analytical views such as:
     - category_performance
     - loss_analysis
     - sales_trend_final

4. 04_business_queries.sql
   - Supports strategic analysis such as:
     - top loss-driving products
     - top profit-generating products
     - profit margin by category

---

## Key Insights Highlighted in the Project

- Technology is a major contributor to total sales and profit
- Certain sub-categories, such as Machines and Tables, contribute significant losses
- A small number of products create disproportionate negative impact on profitability
- Product mix optimization and pricing review can improve margins
- Profitability analysis helps prioritize high-value product lines and reduce exposure to unprofitable items

---

## Dashboard Output

The dashboard summarizes the most important metrics in a visual format, allowing business stakeholders to explore:

- Revenue by category
- Profitability by category
- Loss-making products and sub-categories
- Sales trend over time
- Product-level performance indicators

The exported dashboard files are available in the dashboard folder.

---

## Repository Structure

```text
sales-analytics-dashboard/
├── dashboard/
│   ├── dashboard-screenshot.png
│   └── Dashboard-export.pdf
├── data/
│   └── dataset-source-note.txt
├── sql/
│   ├── 01_data_import_cleaning.sql
│   ├── 02_exploratory_analysis.sql
│   ├── 03_analytical_views.sql
│   └── 04_business_queries.sql
├── README.md
└── .git/
```

---

## Recommended Use

To reproduce the analysis:

1. Import the raw sales source file into MySQL.
2. Run the scripts in the sql folder in sequence.
3. Validate the cleaned dataset and analytical views.
4. Connect the transformed tables to Power BI.
5. Use the dashboard to interpret sales and profitability performance.

---

## Author

Joshua Dominic

Portfolio Project | Data Analytics
