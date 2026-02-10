# Gross Profit Analysis Dashboard (Power BI)

## Overview
An interactive Power BI dashboard developed to analyze **Plant Co.’s gross profit performance**.  
The dashboard provides insights into Year-to-Date (YTD) and Previous Year-to-Date (PYTD) gross profit, regional performance, product category contributions, monthly trends, and profitability segmentation.

It enables stakeholders to identify underperforming regions, seasonal trends, and high-priority accounts for data-driven decision-making.

---

## Tech Stack
- Power BI
- DAX
- Power Query
- Financial Data Modeling

---

## Key Features
- KPI cards for YTD, PYTD, YTD vs PYTD, and GP%
- Regional performance analysis using treemap
- Monthly YTD vs PYTD comparison using bar charts
- Product category analysis (Indoor, Landscape, Outdoor)
- Profitability segmentation using scatter plots
- Interactive slicers and cross-filtering

---

## DAX Highlights
```DAX
YTD_GrossProfit = TOTALYTD([Grossprofit], fact_sales[Date_Time])
YTD vs PYTD = [S_YTD] - [S_PYTD]
GP% = DIVIDE([Grossprofit], [Sales])
