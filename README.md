# Mohd Faizanul Haque

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat&logo=postgresql&logoColor=white)
![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=flat&logo=snowflake&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=flat&logo=databricks&logoColor=white)
![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat&logo=dbt&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![Excel](https://img.shields.io/badge/Excel-217346?style=flat&logo=microsoftexcel&logoColor=white)

### Data Analyst & Analytics Engineer — New Delhi, India

---

## About

I'm a Data Analyst who works comfortably on both sides of the pipeline: building the warehouse layer that makes data trustworthy, and turning that data into findings someone can act on. My toolkit spans **SQL, Python, Power BI, Snowflake, Databricks, and dbt**, developed through a Data Analytics internship and a series of end-to-end analytics projects covering e-commerce, hospitality, retail, and customer behavior.

I care about the same question at every layer of a project: *if a stakeholder built a decision on this number, would it hold up?* That means writing dbt tests that actually fail when data breaks a rule, flagging inconsistencies between dashboard pages before they undermine trust in the whole report, and backing every recommendation with a quantified number rather than a vague direction.

## Table of Contents

- [About](#about)
- [Portfolio Projects](#portfolio-projects)
  - [Olist E-Commerce Analytics Platform](#olist-e-commerce-analytics-platform) — `Databricks · Unity Catalog · dbt · SQL · Power BI`· pyspark
  - [Hotel Analytics Data Warehouse](#hotel-analytics-data-warehouse) — `Snowflake · SQL · Power BI`
  - [Sales Analytics](#sales-analytics) — `Python · Pandas · Excel · Power BI`
  - [Analysis of Customer Behavior](#analysis-of-customer-behavior) — `Python · SQL · Power BI`
- [Skills](#skills)
- [Experience](#experience)
- [Education](#education)
- [Resume](#resume)
- [Contact](#contact)

---

## Portfolio Projects

Olist E-Commerce Analytics Platform

Goal: Build an end-to-end analytics engineering platform that transforms nine raw e-commerce source tables into a governed, business-ready dimensional model for reporting and decision-making.

Code: View Repository

Repository: View Project Repository

Description: This project demonstrates an end-to-end analytics engineering workflow built on Databricks and Unity Catalog, using dbt and following the Medallion Architecture (Bronze, Silver, Gold).

The pipeline ingests raw Olist e-commerce tables into the Bronze layer, preserving the original source data. The Silver layer standardizes types, handles nulls, normalizes strings, and filters invalid records through dbt staging models. The Gold layer transforms the cleaned data into a star schema — a central orders fact table joined to order items, payments, reviews, and customer, product, and seller dimensions.

The curated Gold-layer data connects to Power BI to create dashboards analyzing revenue trends, sales performance, customer behavior, and product performance.

What I Built:

Designed a scalable Bronze → Silver → Gold lakehouse pipeline in Databricks with Unity Catalog governance.
Built reusable dbt transformations for data cleaning, validation, and standardization.
Implemented dbt tests enforcing uniqueness and accepted values on every build.
Modeled a star schema (fact orders, order items, payments, reviews; customer, product, seller, date dimensions).
Connected the Gold layer to Power BI for business intelligence and visualization.
Identified and documented a data-quality inconsistency between two dashboard pages, rather than silently correcting it.

Key Analytics:

Revenue and order trends
Customer segmentation and city-level spend
Product category performance
Payment method behavior
Repeat-customer rate
Review score distribution

Skills: SQL, Python, Data Cleaning, Data Validation, ETL, Data Transformation, Data Warehousing, Data Modeling, Data Quality, Business Intelligence, Data Visualization

Technology: Databricks, Unity Catalog, dbt, Power BI, Medallion Architecture (Bronze, Silver, Gold)

Hotel Analytics Data Warehouse

Goal: Build an end-to-end data engineering and analytics pipeline that transforms raw hotel booking data into clean, validated, and business-ready datasets for reporting and decision-making.

Code: View SQL Pipeline

Repository: View Project Repository

Description: This project demonstrates an end-to-end data engineering workflow built on Snowflake, following the Medallion Architecture (Bronze, Silver, Gold).

The pipeline starts by ingesting raw hotel booking CSV files into the Bronze layer, preserving the original data. The Silver layer performs data cleaning, validation, and standardization, including handling invalid dates, correcting booking status values, validating email formats, normalizing text fields, and converting data types.

The Gold layer transforms the cleaned data into analytics-ready tables, including a booking fact table, daily booking summaries, and city-level revenue aggregations.

The curated Gold-layer data is then connected to Power BI to create interactive dashboards for analyzing revenue trends, booking performance, room types, city-level revenue, and operational KPIs.

What I Built:

Designed a scalable Bronze → Silver → Gold data pipeline in Snowflake.
Built reusable SQL transformations for data cleaning, validation, and standardization.
Implemented data quality checks to identify missing values and inconsistent records.
Created analytics-ready Gold-layer tables and business aggregations.
Developed a clean booking fact table for analytical reporting.
Connected Snowflake data to Power BI for business intelligence and visualization.
Built dashboards to monitor revenue, bookings, room performance, city performance, and operational KPIs.

Key Analytics:

Revenue trends and growth
Booking performance
City-level revenue
Room type performance
Booking cancellations
Operational KPIs

Skills: SQL, Data Cleaning, Data Validation, ETL, Data Transformation, Data Warehousing, Data Modeling, Data Quality, Business Intelligence, Data Visualization

Technology: Snowflake SQL, Power BI, CSV Data Ingestion, Medallion Architecture (Bronze, Silver, Gold)

Analysis of Customer Behavior

Code & Analysis:

View SQL Analysis
View Python Analysis
View Project Repository

Goal: Analyze customer shopping behavior to identify high-value customer segments, purchasing patterns, subscription trends, and discount usage, and translate these findings into actionable business recommendations.

Description: This project analyzes 3,900+ customer transactions using Python, SQL, and Power BI to understand purchasing behavior and identify factors that influence customer value and business performance.

The analysis follows an end-to-end workflow, starting with data preparation and exploratory analysis in Python, followed by business-focused analysis using SQL, and ending with an interactive Power BI dashboard for reporting and visualization.

The analysis examines customer spending, gender-based revenue, subscription behavior, discount usage, product performance, shipping preferences, customer loyalty, and revenue contribution across age groups.

Customers are also segmented into New, Returning, and Loyal groups based on their previous purchase history to better understand customer value and retention patterns.

What I Built:

Cleaned and prepared customer transaction data using Python and Pandas.
Performed exploratory data analysis (EDA) to identify purchasing patterns and trends.
Analyzed 3,900+ customer transactions using SQL.
Used advanced SQL techniques including CTEs, subqueries, CASE statements, aggregate functions, and window functions.
Compared spending and revenue between subscribed and non-subscribed customers.
Identified products with high discount utilization and strong customer demand.
Segmented customers into New, Returning, and Loyal groups based on previous purchases.
Analyzed repeat-buyer subscription behavior to understand potential retention opportunities.
Compared revenue contribution across customer age groups.
Developed an interactive Power BI dashboard to communicate KPIs, customer trends, product performance, and purchasing behavior.

Key Business Questions:

Do subscribed customers spend more than non-subscribers?
Which customer segments generate the most revenue?
Which products have the highest demand and discount usage?
How does customer loyalty relate to subscription behavior?
Which age groups contribute the most revenue?
How does shipping preference relate to average purchase value?
What purchasing patterns can support customer retention strategies?

Key Analytics:

Customer segmentation
Customer spending and revenue analysis
Subscription behavior
Discount utilization
Product performance
Customer loyalty and repeat purchases
Age-group revenue analysis
Shipping behavior
Purchase patterns

Skills: Python, Pandas, SQL, Data Cleaning, Exploratory Data Analysis, Customer Segmentation, CTEs, Subqueries, CASE Statements, Window Functions, Data Visualization, Business Analysis, KPI Reporting

Technology: Python, Pandas, SQL, Power BI, Jupyter Notebook

Sales Analytics

Project Files:

View Python Analysis
View Cleaned Dataset
View Project Repository

Goal: Analyze five years of sales data to identify revenue drivers, profitability trends, seasonal demand patterns, and regional and channel performance, and provide recommendations to support business growth.

Description: This project analyzes 64,000+ sales records across five years to understand sales performance, revenue trends, profitability, seasonal demand, regional performance, and sales-channel behavior.

The project follows an end-to-end data analytics workflow, beginning with data preparation and exploratory analysis in Python, followed by data transformation and preparation for reporting, and ending with an interactive Power BI dashboard.

The analysis focuses on identifying recurring sales patterns, understanding differences across regions and channels, and translating the findings into actionable recommendations for inventory planning, marketing, pricing, product mix, and regional expansion.

What I Built:

Analyzed 64,000+ sales records covering five years.
Cleaned and prepared sales data using Python and Pandas.
Performed exploratory data analysis to identify revenue and sales trends.
Analyzed regional and sales-channel performance.
Identified recurring seasonal patterns, including May–June revenue peaks and January slowdowns.
Evaluated product and profitability trends to identify revenue drivers and business risks.
Prepared cleaned data for visualization and reporting.
Developed an interactive Power BI dashboard to monitor sales KPIs, revenue trends, regional performance, and product performance.
Translated analytical findings into business recommendations for improving sales and profitability.

Key Business Questions:

Which regions and channels generate the strongest sales performance?
Which products are the major revenue drivers?
How does sales performance change over time?
What seasonal patterns can be identified?
Which regions or channels represent potential business risks?
Where are the opportunities for revenue and market growth?
How can inventory, pricing, and marketing strategies be improved?

Key Analytics:

Revenue and sales performance
Regional performance
Sales-channel analysis
Product performance
Profitability trends
Seasonal demand patterns
Revenue drivers
Business growth opportunities

Skills: Python, Pandas, NumPy, Matplotlib, Seaborn, Excel, Data Cleaning, Exploratory Data Analysis, Trend Analysis, Business Analysis, KPI Reporting, Data Visualization

Technology: Python, Excel, Power BI, Pandas, NumPy, Matplotlib, Seaborn

Skills

Languages & Query: SQL, Python, Pandas, NumPy Platforms: Snowflake, Databricks, Unity Catalog Transformation & Modeling: dbt, ETL, Medallion Architecture, Data Warehousing, Data Modeling Visualization: Power BI, Excel, Matplotlib, Seaborn Other: Data Cleaning, Data Validation, Data Quality, Exploratory Data Analysis, Customer Segmentation, Business Analysis, KPI Reporting
---

## Experience

### Full-Stack Developer Intern (Data Analytics)
**MetaCyrus.tech — New Delhi, India**
**July 2024 – September 2024**

- Performed data handling, preprocessing, cleaning, and validation to improve dataset accuracy and reliability.
- Organized and transformed datasets to support reporting workflows and data-driven decision-making.
- Developed reports and dashboards to identify business trends, performance metrics, and operational insights.
- Collaborated with cross-functional teams to understand requirements and deliver analytical solutions aligned with business needs.
- Prepared structured datasets and improved the usability of reporting information.

---

## Education

**Guru Gobind Singh Indraprastha University**
Bachelor of Technology in Computer Science
New Delhi, India
Graduated: July 2026 · CGPA: 7.9

---

## Resume

A detailed resume is available on request — see [Contact](#contact) below.

---

## Contact

📧 **Email:** mdf860111@gmail.com
💻 **GitHub:** [faizan171103](https://github.com/faizan171103)
📍 **New Delhi, India**
