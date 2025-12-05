# ☕ Coffee Shop Sales Analytics Dashboards
### 1. Project Overview

This project presents an end-to-end business intelligence solution built using Power BI and MySQL to analyze sales performance for a coffee shop. The goal of this dashboard is to help stakeholders understand revenue trends, product performance, customer behavior, and operational efficiency through interactive visualizations.


### 2. Key Features of the Dashboard

• Total Sales Overview – Track revenue, transactions, and average order values.

• Product Performance – Identify bestselling products and categories.

• Location-Based Insights – Compare sales performance across shop locations.

• Time Series Analysis – View sales trends by day, month, and hour.

• Customer Behavior – Understand buying patterns and peak business hours.

• Interactive Filters – Slicers for date, product, category, and location help refine analysis.


### 3.Data Source

• Database: MySQL

• Tables Included: Sales Transactions, Products, Store Details, Calendar Table (custom)

• ETL: Data extraction using SQL queries, followed by transformations in Power BI’s Power Query Editor### 3.Data Source



### 4. Tools & Technologies

MySQL (data storage & querying)

Power BI Desktop

Data Modeling (DAX, Relationships)

Data Cleaning & Transformation (Power Query)

Visual Analytics

### 5. Dashboard Features
• Sales Performance Overview

- Total Revenue, Total Orders, Total Quantity Sold

- Daily, Monthly & Yearly trends

- Average order value

 • Product Analytics

- Top-selling products

- Category-wise performance (coffee, bakery, beverages, etc.)

- Low-performing products for strategic improvement

 • Store Performance

- Comparison between different store locations

- Revenue contribution share

- Peak sales days & busiest hours


 • Interactive Visuals

- Slicers for filtering by date, product category, store, etc.

- Tooltips for detailed insights

- Trend lines and KPI cards for at-a-glance summaries

### 6. Data Model

The data model for this project follows a Star Schema design to ensure optimized performance, simplified DAX calculations, and a clean relational structure.

**Fact Table — Coffee Shop Sales**

This is the central table in the model and contains all transactional data

This table records every sale made across different coffee shop locations and products.

2. Dimension Table — Date Table

A dedicated calendar table used to support time-intelligence calculations.
It contains fields such as:

- Date

- Day Name

- Day No

- Month & Year

- Month Name

The Date Table has a one-to-many (1:*) relationship with the transaction_date field in the fact table, allowing accurate filtering and time-based analysis.

3. Measures Table

A separate table created solely for storing DAX measures (e.g., Above Avg Bars).
This table does not participate in relationships but helps keep the model clean and organized by separating calculations from raw data.

⭐ Schema Type — Star Schema

The model forms a classic Star Schema where:

The Coffee Shop Sales table is the central fact table

The Date Table is a supporting dimension table

The Measures Table provides semantic structure for KPIs

This structure ensures efficient querying, enhanced readability, and strong performance within Power BI.



### 4. Insights & Findings

Some key insights uncovered from the analysis:

Weekends show higher sales volume compared to weekdays.

Peak hours fall between 8 AM – 11 AM, driven by breakfast and morning coffee.

Certain product categories (e.g., coffee and pastries) dominate revenue.

Specific store locations consistently outperform others.

### 6.	Screenshots / Demos

![Dashboard Preview](https://github.com/rakeshjetty2000-alt/Coffee-Shop-Sales/blob/main/Coffee%20Shop%20Sales%20.png)

5. Dashboard Preview

(Add screenshots in /Assets folder and reference them here)

Example:https://github.com/rakeshjetty2000-alt/Coffee-Shop-Sales/blob/main/Coffee%20Shop%20Sales%20.png
