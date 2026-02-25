# E-Commerce Sales Dashboard (Power BI | MS SQL Server)

## Overview
This project is an end-to-end **E-Commerce Sales Dashboard** built in **Power BI** using data stored in **MS SQL Server**.  
The dashboard helps stakeholders track **Year-To-Date (YTD)** performance, compare it with **Previous Year-To-Date (PYTD)**, and identify trends across **categories, regions, states, products, and shipping types**.

### Quick Summary
This dashboard tracks **YTD vs PYTD** performance and highlights **YoY trends**, enabling stakeholders to identify profit/margin changes, category winners/losers, regional performance, and shipping contribution for faster decisions.

## Dashboard Overview
![E-Commerce Sales Dashboard](assets/dashboard-overview.png)

### Key Business Snapshot (from dashboard)
- **YTD Sales:** $11.53M (YoY: -0.83%)
- **YTD Profit:** $1.34M (YoY: +4.50%)
- **YTD Quantity:** 107.2K (YoY: -7.29%)
- **YTD Profit Margin:** 11.58% (YoY: +5.37%)

---

## Problem Statement
A US-based e-commerce company needed a single interactive dashboard to:
- Monitor overall business performance using key KPIs
- Compare current year performance against previous year
- Identify top-performing and low-performing products
- Understand regional/state-level sales distribution
- Analyze shipping type contribution to sales
- Track monthly trends for sales, profit, quantity, and profit margin

## Objectives
The dashboard was designed to answer these core questions:
- What are the **YTD Sales, YTD Profit, YTD Quantity, and YTD Profit Margin**?
- How is performance changing **YoY (Year-on-Year)**?
- Which **Category** is growing/declining in **YTD vs PYTD**?
- Which **States** contribute the most sales?
- What are the **Top 5** and **Bottom 5** products by **YTD Sales**?
- Which **Region** is strongest/weakest by sales contribution?
- Which **Shipping Type** contributes the most to sales?

---

## Data & Tools Used
### Data Source
- **MS SQL Server** (database used as the source for Power BI)

### Tools
- **Power BI Desktop**
- **Power Query** (ETL: cleaning + transformation)
- **DAX** (measures + time intelligence)
- **Data Modeling** (relationships + date table)

---

## Approach (End-to-End Workflow)
1. Imported and stored data in **MS SQL Server**
2. Connected **Power BI** to SQL Server (data import)
3. Cleaned and transformed data using **Power Query**
   - Fixed data types
   - Handled missing values where needed
   - Standardized columns for reporting
4. Built a clean **data model**
   - Fact table for transactions
   - Dimension tables for slicing (Product, Geography/State, Region, Segment, Ship Type)
   - Created a dedicated **Date Table** for time intelligence
5. Created key **DAX measures**
   - YTD, PYTD, YoY %, Profit Margin, trend logic
   - Ranking measures for Top/Bottom products
6. Designed the dashboard with clear layout & interactivity
   - KPI cards + sparklines
   - Category comparison charts
   - State map
   - Region contribution
   - Shipping type breakdown
   - Top/Bottom products visuals

---

## Key KPIs (Implemented)
- YTD Sales
- YTD Profit
- YTD Quantity
- YTD Profit Margin
- PYTD (Previous Year-To-Date) for comparison
- YoY % Change for each KPI
- Monthly Trend (sparkline-style trend visualization)

---

## Dashboard Features
1) **KPI Summary + Trend**  
Quick view of business health with YoY indicators and monthly performance trend.

2) **Category Performance**  
Category-wise comparison using **YTD vs PYTD** and **YoY % Change**.

3) **Sales by State (Map)**  
State-level sales visualization to identify strong and weak geographic markets.

4) **Top & Bottom Products**  
Top 5 and Bottom 5 products by YTD Sales to support product prioritization decisions.

5) **Regional Contribution**  
Region-wise YTD sales and percentage contribution to identify strongest and weakest regions.

6) **Shipping Type Analysis**  
YTD Sales by shipping mode with % contribution to understand shipping preferences and operational impact.

---

## Insights (From Dashboard)
- Sales are slightly down YoY, but profit and profit margin improved, showing better profitability.
- Quantity declined more than sales, which may indicate product mix change or pricing impact.
- Office Supplies contributes the highest sales, so even small changes here strongly impact total revenue.
- West region contributes the most, while South region contributes the least, highlighting expansion opportunity.
- Standard Class dominates shipping share, so improving this mode can create the biggest operational ROI.

## Recommendations
- Focus on improving **South** region performance by replicating high-performing region strategies.
- Investigate **quantity decline** drivers (pricing, product mix, or demand shift) and address with targeted campaigns.
- Optimize **Standard Class shipping** since it contributes the highest share of sales.

---

## How to Use
- Use the **Segment** buttons (Consumer / Corporate / Home Office) to filter analysis.
- Use **Region** and other filters to drill down.
- Track KPIs first, then move to Category/Region/State/Product/Shipping insights.
