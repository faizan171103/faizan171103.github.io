# faizan171103.github.io
# Mohd Faizanul Haque - Data Analyst Portfolio

## About

Hi, I'm Mohd Faizanul Haque, a Data Analyst based in New Delhi, India. I have hands-on experience working with SQL, Python, Power BI, Snowflake, and Excel, gained through my Data Analytics internship and multiple end-to-end analytics projects.

I enjoy working with data from the initial stages of data cleaning, preprocessing, and validation through to analysis, data modeling, and visualization. I am particularly interested in using data to uncover trends, answer business questions, and support data-driven decision-making.

My experience includes building ETL pipelines, data warehouses, analytical data models, SQL queries, and interactive Power BI dashboards. I have worked on projects involving hotel bookings, customer behavior, sales performance, revenue analysis, and operational KPIs.

This repository showcases my Data Analytics projects, technical skills, and experience.

## Table of Contents

- [About](#about)
- [Portfolio Projects](#portfolio-projects)
  - [Hotel Analytics Data Warehouse](#hotel-analytics-data-warehouse)
  - [Analysis of Customer Behavior](#analysis-of-customer-behavior)
  - [Sales Analytics](#sales-analytics)
- [Skills](#skills)
- [Experience](#experience)
- [Education](#education)
- [Resume](#resume)
- [Contact](#contact)

---
## Hotel Analytics Data Warehouse

**Goal:** Build an end-to-end data engineering and analytics pipeline that transforms raw hotel booking data into clean, validated, and business-ready datasets for reporting and decision-making.

**Code:** [View SQL Pipeline](https://github.com/faizan171103/snowflake_bookings_analytics/blob/main/bookings_analystics.sql)

**Repository:** [View Project Repository](https://github.com/faizan171103/snowflake_bookings_analytics)

**Description:**  
This project demonstrates an end-to-end data engineering workflow built on **Snowflake**, following the **Medallion Architecture (Bronze, Silver, Gold)**.

The pipeline starts by ingesting raw hotel booking CSV files into the **Bronze layer**, preserving the original data. The **Silver layer** performs data cleaning, validation, and standardization, including handling invalid dates, correcting booking status values, validating email formats, normalizing text fields, and converting data types.

The **Gold layer** transforms the cleaned data into analytics-ready tables, including a booking fact table, daily booking summaries, and city-level revenue aggregations.

The curated Gold-layer data is then connected to **Power BI** to create interactive dashboards for analyzing revenue trends, booking performance, room types, city-level revenue, and operational KPIs.

**What I Built:**
- Designed a scalable **Bronze → Silver → Gold** data pipeline in Snowflake.
- Built reusable **SQL transformations** for data cleaning, validation, and standardization.
- Implemented data quality checks to identify missing values and inconsistent records.
- Created analytics-ready Gold-layer tables and business aggregations.
- Developed a clean booking fact table for analytical reporting.
- Connected Snowflake data to **Power BI** for business intelligence and visualization.
- Built dashboards to monitor revenue, bookings, room performance, city performance, and operational KPIs.

**Key Analytics:**
- Revenue trends and growth
- Booking performance
- City-level revenue
- Room type performance
- Booking cancellations
- Operational KPIs

**Skills:**  
SQL, Data Cleaning, Data Validation, ETL, Data Transformation, Data Warehousing, Data Modeling, Data Quality, Business Intelligence, Data Visualization

**Technology:**  
Snowflake SQL, Power BI, CSV Data Ingestion, Medallion Architecture (Bronze, Silver, Gold)

## Customer Behavior Analysis

**Code & Analysis:**

- [View SQL Analysis](https://github.com/faizan171103/analysis_of_customer_behaviors/blob/main/customer_behavior_analysis.sql)
- [View Python Analysis](https://github.com/faizan171103/analysis_of_customer_behaviors/blob/main/customer_behavior_of_shopping.ipynb)
- [View Project Repository](https://github.com/faizan171103/analysis_of_customer_behaviors)

**Goal:** Analyze customer shopping behavior to identify high-value customer segments, purchasing patterns, subscription trends, and discount usage, and translate these findings into actionable business recommendations.

**Description:**  
This project analyzes **3,900+ customer transactions** using Python, SQL, and Power BI to understand purchasing behavior and identify factors that influence customer value and business performance.

The analysis follows an end-to-end workflow, starting with **data preparation and exploratory analysis in Python**, followed by business-focused analysis using **SQL**, and ending with an interactive **Power BI dashboard** for reporting and visualization.

The analysis examines customer spending, gender-based revenue, subscription behavior, discount usage, product performance, shipping preferences, customer loyalty, and revenue contribution across age groups.

Customers are also segmented into **New, Returning, and Loyal** groups based on their previous purchase history to better understand customer value and retention patterns.

**What I Built:**
- Cleaned and prepared customer transaction data using **Python and Pandas**.
- Performed exploratory data analysis (EDA) to identify purchasing patterns and trends.
- Analyzed **3,900+ customer transactions** using SQL.
- Used advanced SQL techniques including **CTEs, subqueries, CASE statements, aggregate functions, and window functions**.
- Compared spending and revenue between subscribed and non-subscribed customers.
- Identified products with high discount utilization and strong customer demand.
- Segmented customers into **New, Returning, and Loyal** groups based on previous purchases.
- Analyzed repeat-buyer subscription behavior to understand potential retention opportunities.
- Compared revenue contribution across customer age groups.
- Developed an interactive **Power BI dashboard** to communicate KPIs, customer trends, product performance, and purchasing behavior.

**Key Business Questions:**
- Do subscribed customers spend more than non-subscribers?
- Which customer segments generate the most revenue?
- Which products have the highest demand and discount usage?
- How does customer loyalty relate to subscription behavior?
- Which age groups contribute the most revenue?
- How does shipping preference relate to average purchase value?
- What purchasing patterns can support customer retention strategies?

**Key Analytics:**
- Customer segmentation
- Customer spending and revenue analysis
- Subscription behavior
- Discount utilization
- Product performance
- Customer loyalty and repeat purchases
- Age-group revenue analysis
- Shipping behavior
- Purchase patterns

**Skills:**  
Python, Pandas, SQL, Data Cleaning, Exploratory Data Analysis, Customer Segmentation, CTEs, Subqueries, CASE Statements, Window Functions, Data Visualization, Business Analysis, KPI Reporting

**Technology:**  
Python, Pandas, SQL, Power BI, Jupyter Notebook

## Sales Analytics

**Project Files:**

- [View Python Analysis](https://github.com/faizan171103/sales_analytics/blob/main/sales_analytics.ipynb)
- [View Cleaned Dataset](https://github.com/faizan171103/sales_analytics/blob/main/Sales_data_after_EDA.csv)
- [View Project Repository](https://github.com/faizan171103/sales_analytics)

**Goal:** Analyze five years of sales data to identify revenue drivers, profitability trends, seasonal demand patterns, and regional and channel performance, and provide recommendations to support business growth.

**Description:**  
This project analyzes **64,000+ sales records across five years** to understand sales performance, revenue trends, profitability, seasonal demand, regional performance, and sales-channel behavior.

The project follows an end-to-end data analytics workflow, beginning with data preparation and exploratory analysis in **Python**, followed by data transformation and preparation for reporting, and ending with an interactive **Power BI dashboard**.

The analysis focuses on identifying recurring sales patterns, understanding differences across regions and channels, and translating the findings into actionable recommendations for inventory planning, marketing, pricing, product mix, and regional expansion.

**What I Built:**
- Analyzed **64,000+ sales records covering five years**.
- Cleaned and prepared sales data using **Python and Pandas**.
- Performed exploratory data analysis to identify revenue and sales trends.
- Analyzed regional and sales-channel performance.
- Identified recurring seasonal patterns, including **May–June revenue peaks and January slowdowns**.
- Evaluated product and profitability trends to identify revenue drivers and business risks.
- Prepared cleaned data for visualization and reporting.
- Developed an interactive **Power BI dashboard** to monitor sales KPIs, revenue trends, regional performance, and product performance.
- Translated analytical findings into business recommendations for improving sales and profitability.

**Key Business Questions:**
- Which regions and channels generate the strongest sales performance?
- Which products are the major revenue drivers?
- How does sales performance change over time?
- What seasonal patterns can be identified?
- Which regions or channels represent potential business risks?
- Where are the opportunities for revenue and market growth?
- How can inventory, pricing, and marketing strategies be improved?

**Key Analytics:**
- Revenue and sales performance
- Regional performance
- Sales-channel analysis
- Product performance
- Profitability trends
- Seasonal demand patterns
- Revenue drivers
- Business growth opportunities

**Skills:**  
Python, Pandas, NumPy, Matplotlib, Seaborn, Excel, Data Cleaning, Exploratory Data Analysis, Trend Analysis, Business Analysis, KPI Reporting, Data Visualization

**Technology:**  
Python, Excel, Power BI, Pandas, NumPy, Matplotlib, Seaborn


# Experience

## Full-Stack Developer Intern (Data Analytics)

**MetaCyrus.tech — New Delhi, India**  
**July 2024 – September 2024**

- Performed data handling, preprocessing, cleaning, and validation to improve dataset accuracy and reliability.
- Organized and transformed datasets to support reporting workflows and data-driven decision-making.
- Developed reports and dashboards to identify business trends, performance metrics, and operational insights.
- Collaborated with cross-functional teams to understand requirements and deliver analytical solutions aligned with business needs.
- Prepared structured datasets and improved the usability of reporting information.

---

# Education

## Guru Gobind Singh Indraprastha University

**Bachelor of Technology in Computer Science**  
New Delhi, India

**Graduated: July 2026**

**CGPA: 7.9**
# Contact

📧 **Email:** mdf860111@gmail.com

💻 **GitHub:** [faizan171103](https://github.com/faizan171103)

📍 **New Delhi, India**



