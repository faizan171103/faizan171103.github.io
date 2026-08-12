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


