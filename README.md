# Business Intelligence Dashboard - Superstore Sales Analysis

## Overview
End-to-end Business Intelligence project analyzing 9,800 Superstore sales transactions
using Python for data preparation and Power BI for interactive dashboard visualization.
This project demonstrates the full BI workflow from raw data cleaning to professional
executive dashboard design.

## Objectives
- Clean and prepare raw sales data for Business Intelligence analysis
- Engineer new features to enrich the dataset for deeper insights
- Build an interactive Power BI dashboard revealing key business insights
- Analyze sales performance across regions, categories, time and customer segments
- Identify top performing products and underperforming areas for business action

## Tools Used
- Python
- Pandas
- Power BI Desktop
- VS Code
- Git and GitHub

## Dataset
- Source: Superstore Sales Dataset (Kaggle)
- Size: 9,800 rows and 18 original columns
- After preparation: 9,800 rows and 24 columns
- Coverage: 4 years of global superstore sales transactions

---

## Project Structure
1. Data Preparation (Python)
2. Feature Engineering (Python)
3. Interactive Dashboard (Power BI)

---

## Phase 1 - Data Preparation

### Step 1 - Data Loading and Exploration
Loaded 9,800 rows of Superstore sales data containing 18 columns covering
order details, customer information, product categories and sales figures.

### Step 2 - Missing Value Treatment
Identified 11 missing values in the Postal Code column.
Filled missing values with 0 since Postal Code is not used in dashboard analysis.
All other columns had no missing values confirming a relatively clean dataset.

### Step 3 - Date Column Conversion
Order Date and Ship Date columns were stored as plain text objects.
Converted both columns to proper datetime format using dayfirst=True
to handle the day/month/year date format in this dataset.
This conversion is essential for all time based analysis in Power BI.

### Step 4 - Time Feature Engineering
Extracted the following new columns from Order Date to enable time based analysis:
- Year — for annual sales trend analysis
- Month — for monthly performance tracking
- Month Name — for readable chart labels in Power BI
- Quarter — for quarterly business review analysis

### Step 5 - Shipping Performance Feature
Calculated Days to Ship by finding the difference between Ship Date and Order Date.
Average shipping time across all orders: 4.0 days.
This metric enables delivery performance analysis across ship modes and regions.

### Step 6 - Sales Category Feature
Categorized each order into sales size buckets:
- Small: $0 to $100
- Medium: $100 to $500
- Large: $500 to $1,000
- Very Large: $1,000 to $10,000

This segmentation makes it easier to analyze order patterns and
identify which customer segments drive the most revenue.

### Step 7 - Export for Power BI
Saved the cleaned and enriched dataset as superstore_cleaned.csv
with 24 columns ready for direct import into Power BI Desktop.

---

## Feature Engineering Summary

| New Column | Description | Purpose |
|---|---|---|
| Year | Extracted from Order Date | Annual trend analysis |
| Month | Extracted from Order Date | Monthly performance |
| Month Name | Extracted from Order Date | Readable chart labels |
| Quarter | Extracted from Order Date | Quarterly reviews |
| Days to Ship | Ship Date minus Order Date | Delivery performance |
| Sales Category | Sales bucketed into 4 tiers | Order size analysis |

---

## Key Observations from Data Preparation
- Dataset covers 4 years of sales transactions with no gaps in key columns
- Average delivery time of 4.0 days across all ship modes
- Sales range from very small orders under $100 to very large orders over $1,000
- No missing values in any sales or category columns ensuring reliable analysis

---

## Phase 2 - Power BI Dashboard

### Dashboard Visuals
Six interactive visuals were built to analyze superstore sales performance:

1. **Total Sales KPI Card** — Headline revenue figure of $2.26M across 4 years
2. **Sales by Region** — West region leads with highest sales, South has lowest
3. **Sales by Category** — Technology dominates at $827K, followed by Furniture
   and Office Supplies
4. **Sales Trend by Month** — Clear seasonality pattern with peaks in
   September to November across all years driven by holiday shopping
5. **Sales by Customer Segment** — Consumer segment leads with over $1M,
   Home Office generates the least
6. **Top 10 Products** — Canon imageCLASS is the hero product with sales
   far exceeding all other products

### Interactive Feature
Year slicer allows filtering all visuals simultaneously by year
enabling year over year performance comparison with one click.

### Key Business Insights
- West region should receive highest marketing investment given sales dominance
- Technology category is the strongest revenue driver
- Business shows healthy year over year growth from 2015 to 2018
- Sales consistently peak in Q4 — inventory and staffing should be planned accordingly
- Canon imageCLASS is a hero product — ensuring stock availability is critical
- Consumer segment drives the majority of revenue — retention campaigns are essential
- January and February are slowest months — targeted promotions needed to boost sales

---

## Project Status
✅ Data loading and exploration complete
✅ Missing value treatment complete
✅ Date conversion complete
✅ Time feature engineering complete
✅ Shipping performance feature complete
✅ Sales category feature complete
✅ Cleaned dataset exported for Power BI
✅ Power BI dashboard complete - 6 interactive visuals
✅ Year slicer for interactive filtering
✅ Dashboard exported as PDF and screenshot

---

## Connection to Portfolio
This project builds on skills developed in previous projects:
- E-Commerce Data Analysis (Python, Pandas, Matplotlib, Scikit-learn)
- Sentiment Analysis NLP project (Python, NLTK, Logistic Regression)

This project adds Business Intelligence and interactive dashboard skills
to complete a well rounded data science and analytics portfolio.

---

## Author
Patricia Kiarie | Data Science Undergraduate
Passionate about using data to drive business strategy and decision making
Tools: Python, Pandas, Power BI, Scikit-learn, NLTK, Google Colab, VS Code
Currently exploring the intersection of Data Science, Business and AI