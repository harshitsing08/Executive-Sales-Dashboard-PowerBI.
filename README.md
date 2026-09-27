# 📊 Executive Sales Dashboard — Power BI Project

An end-to-end Business Intelligence project built in Power BI, covering data modeling, advanced DAX, customer segmentation, and executive-level dashboard design and storytelling.

## 🎯 Project Overview

This dashboard helps sales leadership get a unified view of regional performance, customer profitability, and growth trends to guide marketing and retention decisions.

## 🗂️ Dataset

- **Source:** Excel dataset — 3 related tables (Orders, Customers, Products) + a custom Calendar table built with DAX
- **Time period:** Jan 2023 – Dec 2024
- **Size:** Orders: 1,200 rows · Customers: 40 rows · Products: 52 rows

## 🛠️ Tools & Skills Used

- Power BI Desktop
- DAX (RANKX, CALCULATE, SWITCH, SAMEPERIODLASTYEAR)
- Power Query (data cleaning & transformation)
- What-if Parameters (dynamic Top N filtering)
- Power BI Service (publishing)

## 📐 Data Model

A star-schema model with `Orders` as the fact table, related to `Customers`, `Products`, and a `Calendar` dimension table — all single-direction, many-to-one relationships for optimal performance.

## 🧮 Key DAX Measures

| Measure | Purpose |
|---|---|
| **Customer Rank** | Ranks customers by total sales to surface top/bottom performers |
| **Top N Sales** | Lets the viewer dynamically choose Top 5/10/20 customers |
| **Customer Segment** | Buckets customers into High / Medium / Low value by profit |
| **YoY Growth %** | Shows year-over-year sales growth trend |

## 📈 Dashboard Pages

1. **Executive Overview** — KPI cards (Total Sales, Profit, Margin, YoY Growth, Orders), sales trend, regional and category performance
2. **Customer Analysis** — Top N customer ranking, profit-based segmentation, customer-level detail table
3. **Business Insights** — Executive storytelling section with key findings and strategic recommendations

## 💡 Key Business Insights

- **Key Growth Insight:** Sales grew 112% year-over-year, with consistent monthly performance between 120K–160K
- **Underperforming Region:** North region trails all other regions in total sales, indicating an opportunity for targeted marketing
- **Most Profitable Category:** Office Supplies leads in profit contribution, followed by Furniture and Technology
- **Customer Concentration Risk:** Top 10 customers contribute about 35–36% of total sales revenue, creating moderate dependency risk

## ✅ Strategic Recommendations

- Increase marketing focus in the North region to close the performance gap with other regions
- Introduce a customer loyalty program to diversify the customer base and reduce dependency on the top 10 customers

## ⚡ Performance Optimizations

- Hid unused ID columns from report view while keeping them for relationships
- Verified all relationships are single-direction (many-to-one) to avoid unnecessary filter propagation
- Split visuals across multiple pages instead of overloading a single page
- Used measures instead of calculated columns wherever possible

## 🔗 Live Dashboard

👉 [View the published dashboard on Power BI Service](https://app.powerbi.com/groups/me/reports/1bf4c7ea-bdf2-42d3-a550-440418b6e2f4/f03d49add823e1a646b5?experience=power-bi)

## 📄 Full Case Study

See [`Portfolio_Case_Study_FINAL.docx`](./Portfolio_Case_Study_FINAL.docx) in this repository for the complete write-up, including business problem, data cleaning steps, and learning outcomes.
