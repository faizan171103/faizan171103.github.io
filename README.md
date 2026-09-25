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
  - [Olist E-Commerce Analytics Platform](#olist-e-commerce-analytics-platform) — `Databricks · Unity Catalog · dbt · SQL · Power BI`
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

### Olist E-Commerce Analytics Platform

**Goal:** Build a governed lakehouse that transforms nine raw Brazilian e-commerce tables into a dimensional model capable of supporting reliable, repeatable business reporting.

**Code:** [View Repository](https://github.com/faizan171103/olist-databricks-lakehouse)

**Stack:** Databricks · Unity Catalog · dbt · SQL · Power BI · Medallion Architecture (Bronze/Silver/Gold)

Raw data lands untouched in Bronze, is standardized and validated in Silver, and rolls up into a proper star schema in Gold — `fact_orders`, `fact_order_items`, `fact_payments`, `fact_reviews` joined against `dim_customers`, `dim_products`, `dim_sellers`, and `dim_date`. dbt tests enforce uniqueness and accepted-value constraints as part of every build, not as an afterthought.

**Key Analytics:**
- **Retention diagnostics** — isolated a **3.05% repeat-customer rate** across 96K customers as the single highest-leverage metric in the dataset
- **Category resilience analysis** — confirmed no single category exceeds 9.26% of revenue, ruling out concentration risk
- **Geographic value mapping** — separated customer *volume* (São Paulo, Rio de Janeiro) from customer *value* (smaller high-spend cities like Loreto), a split a volume-only view would miss entirely
- **Cross-page consistency audit** — caught and documented a real semantic drift between two dashboard pages' "top category" answers, before it could mislead a stakeholder
- **dbt-enforced data quality** — automated uniqueness and accepted-value tests on `customer_id`, `order_id`, `product_id`, `order_status`, and `review_score`, run on every build

**Recommendation highlight:** Prioritize a repeat-purchase/retention model over any single-category optimization — at this AOV and order volume, moving repeat rate even a few points outweighs most acquisition-channel work.

---

### Hotel Analytics Data Warehouse

**Goal:** Build an end-to-end Snowflake pipeline that turns raw hotel booking CSVs into business-ready datasets for revenue, occupancy, and operational reporting.

**Code:** [View Repository](https://github.com/faizan171103/snowflake_bookings_analytics)

**Stack:** Snowflake SQL · Medallion Architecture (Bronze/Silver/Gold) · Power BI

Silver-layer transformations target specific, named failure modes rather than a generic cleaning pass — invalid dates, inconsistent booking-status values, malformed emails, and mixed data types are each handled explicitly, landing in a clean booking fact table plus daily and city-level aggregation tables in Gold.

**Key Analytics:**
- **Cancellation & no-show diagnostics** — quantified a **58.2% combined failure rate** into an estimated **$230K** in unrealized revenue
- **Booking-value ceiling analysis** — found no booking clears $600 against a $332.26 average, exposing a missing premium tier
- **Room-type demand mix** — confirmed a near-even 34/33/32 split across Suite/Standard/Deluxe, ruling out price-driven preference and pointing to real upsell headroom
- **City-level revenue concentration** — isolated five cities carrying consistent, repeatable volume against a long tail of near-zero markets
- **Data-quality flagging** — traced a `(Blank)` gap in booking status and room type back to Silver before it could quietly bias segmentation

**Recommendation highlight:** Attack the cancellation/no-show rate first — deposits, confirmation reminders, and a tiered cancellation policy. Recovering even 10 points of that rate is worth an estimated $40K without acquiring a single new guest.

---

### Sales Analytics

**Goal:** Analyze five years and 64,000+ sales records to identify revenue drivers, profitability trends, and regional/channel performance, and translate the findings into growth recommendations.

**Code:** [View Repository](https://github.com/faizan171103/sales_analytics)

**Stack:** Python · Pandas · NumPy · Matplotlib · Seaborn · Excel · Power BI

An end-to-end Python-to-Power BI workflow: cleaning and EDA in a notebook, a validated CSV export, and a three-page executive dashboard covering trends, product/channel performance, and geographic customer insights.

**Key Analytics:**
- **Channel profitability analysis** — found the Export channel generates only 14.6% of revenue but posts the **highest margin of the three channels (38.01%)**, exposing that the largest channel (Wholesale) is the least margin-efficient
- **Revenue-vs-margin product audit** — identified that the two biggest revenue products (Product 26, Product 25) don't appear among the top-margin products, separating volume drivers from profit drivers
- **Price-margin correlation testing** — confirmed profit margin does *not* track unit price the way expected, ruling out pricing tier as the primary margin driver
- **Customer concentration check** — verified top-5 customer revenue sits under 5% of total revenue, confirming low concentration risk
- **Regional performance mapping** — quantified California at 19.5% of total revenue (nearly double the next state) while isolating Northeast as the one region trailing meaningfully behind the rest

**Recommendation highlight:** Shift investment toward the Export channel and audit pricing on the two highest-revenue, non-top-margin products — both are higher-leverage moves than trying to grow any single category further.

---

### Analysis of Customer Behavior

**Goal:** Analyze 3,900+ customer transactions to identify high-value segments, purchasing patterns, subscription trends, and discount usage, and turn the findings into retention-focused recommendations.

**Code:** [SQL Analysis](https://github.com/faizan171103/analysis_of_customer_behaviors/blob/main/customer_behavior_analysis.sql) · [Python Analysis](https://github.com/faizan171103/analysis_of_customer_behaviors/blob/main/customer_behavior_of_shopping.ipynb) · [Repository](https://github.com/faizan171103/analysis_of_customer_behaviors)

**Stack:** Python · Pandas · SQL (CTEs, subqueries, window functions) · Power BI

A three-stage workflow — Python for cleaning and EDA, SQL for business-focused segmentation and loyalty analysis, Power BI for the interactive dashboard — segmenting customers into New, Returning, and Loyal groups to understand retention drivers.

**Key Analytics:**
- **Subscription-gap quantification** — isolated the **73% non-subscribed majority** as the single largest, zero-acquisition-cost growth lever in the dataset
- **Category-reliance audit** — measured Clothing and Accessories at 70%+ of category revenue, exposing over-reliance on two of four categories
- **Demographic breadth testing** — confirmed sales split close to evenly by gender and across age groups, ruling out narrow targeting as the right strategy
- **New/Returning/Loyal segmentation** — built customer tiers directly from purchase history using SQL window functions, rather than relying on a single lifetime-value number
- **Data-completeness check** — flagged a four-state location panel as a likely truncated view, applying a data-quality caveat before trusting the "top location" finding

**Recommendation highlight:** Launch a subscription-conversion campaign targeting the 73% non-subscribed base — the highest-leverage move available, since it compounds against an already-solid average purchase amount without new acquisition cost.

---

## Skills

| Category | Tools & Techniques |
|---|---|
| **Data Warehousing & Modeling** | Snowflake, Databricks, Unity Catalog, dbt, Medallion Architecture (Bronze/Silver/Gold), Dimensional/Star Schema |
| **Languages** | SQL (CTEs, subqueries, window functions, CASE logic), Python (Pandas, NumPy) |
| **Data Quality & Testing** | dbt tests, data validation, uniqueness & accepted-value constraints, reproducibility auditing |
| **Visualization & BI** | Power BI, Matplotlib, Seaborn, interactive dashboard design |
| **Analysis** | Exploratory Data Analysis, customer segmentation, cohort/retention thinking, trend and seasonality analysis |
| **Tools** | Excel, Jupyter Notebook, Git/GitHub |

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
