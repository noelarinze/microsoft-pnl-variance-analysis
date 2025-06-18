# Microsoft P&L Variance Analysis

Table of Content
- [Project Overview](https://github.com/noelarinze/microsoft-pnl-variance-analysis/edit/main/README.md#Project-Overview) 
- [Data source](https://github.com/noelarinze/microsoft-pnl-variance-analysis/edit/main/README.md#Data-source)
- [Tools](https://github.com/noelarinze/microsoft-pnl-variance-analysis/edit/main/README.md#tools)
- [Exploratory data analysis](https://github.com/noelarinze/microsoft-pnl-variance-analysis/edit/main/README.md#exploratory-data-analysis)
- [Data analysis](https://github.com/noelarinze/microsoft-pnl-variance-analysis/edit/main/README.md#data-analysis)
- [Results](https://github.com/noelarinze/microsoft-pnl-variance-analysis/edit/main/README.md#results)
- [Recommendations](https://github.com/noelarinze/microsoft-pnl-variance-analysis/edit/main/README.md#recommendations)

## Project Overview

This project analyzes Microsoft’s Q1 FY2023 financial performance compared to Q1 FY2022 using actual 10-Q SEC filing data. The goal was to perform a variance analysis that helps stakeholders understand revenue growth, cost shifts, and profitability changes at a glance. The insights derived from this analysis enable executives and investors to assess financial health, spot risk areas, and identify strategic focus points for the next fiscal quarter.

## Data Source

The financial data used in this analysis was sourced from Microsoft Corporation’s official 10-Q quarterly filing submitted to the U.S. Securities and Exchange Commission (SEC) for the fiscal quarter ending September 30, 2022. This filing includes detailed income statement figures that allow for precise comparison against the same quarter in the prior fiscal year (Q1 FY2022).
	•	Access link: https://www.sec.gov/ix?doc=/Archives/edgar/data/789019/000156459022035087/msft-10q_20220930.htm  
	•	File format used: Excel table extracted from the SEC website for comparative analysis.
	•	Structure: Includes line items for revenue, cost of revenue, operating income, R&D, taxes, and earnings per share across Q1 FY2023 and Q1 FY2022.

This reliable source ensured accurate year-over-year variance calculations and trustworthy financial insights for stakeholders.

## Tools

This project was executed using the following tools:
	•	Excel
Used for structuring the raw financial data, calculating year-over-year and budget variances, and building initial visualizations. Excel formulas were also used for financial ratio analysis such as:
	•	Gross Margin % = Gross Margin / Total Revenue
	•	Operating Income % = Operating Income / Total Revenue
	•	Net Income % = Net Income / Total Revenue
	•	Power BI
Employed to design a dynamic financial dashboard with KPIs, variance visuals (bar chart, waterfall), and slicers for interactive exploration. This enabled storytelling with data in a format familiar to business users and executives.
	•	SEC EDGAR Database
Official data source from which Microsoft’s 10-Q filing was accessed and extracted.

# Dashboards 
This Project includes two dashboards:
1. Excel Dashboard for fast P&L visualization and Variance breakdown
2. Power Bi Dashboard for interatctive dep-dive and stakeholder-ready reporting

These tools combined to create a comprehensive financial analysis that is both technically sound and visually insightful.

## Exploratory Data Analysis

The first step was to structure the raw financial data extracted from Microsoft’s 10-Q report. This included organizing Q1 FY2023 and Q1 FY2022 figures side-by-side for a clear comparison of performance.

Key actions taken during the EDA phase:
	•	Cleaned the raw income statement by removing non-numeric values and standardizing rows such as Revenue, Cost of Revenue, Operating Income, and Net Income.
	•	Added computed metrics such as:
	•	Gross Margin = Total Revenue – Total Cost of Revenue
	•	Variance (YoY) = (2023 value – 2022 value) / 2022 value × 100
	•	Calculated performance ratios to provide context to revenue and profit levels.
	•	Verified unusual values — such as the very low provision for income taxes — by cross-checking them against the official filing.

This foundational step ensured that all downstream analysis and visualizations were based on clean, accurate, and interpretable data.

## Data Analysis & Results

Results

The financial results highlight Microsoft’s performance across core revenue streams, profitability, and operational efficiency between Q1 FY2023 and Q1 FY2022. While growth was achieved in several key areas, some underlying shifts suggest opportunities for strategic realignment and operational tightening.

# Chapter 1: Revenue Performance

Microsoft recorded a 10.6% year-over-year revenue growth, rising from $45.3B to $50.1B. This growth was primarily fueled by a 19.9% surge in service and other revenue, signaling Microsoft’s successful transition toward cloud-based and recurring income streams. However, product revenue declined by 5.3%, potentially reflecting softened hardware or traditional software sales.

Insight: The shift toward service-driven growth validates Microsoft’s long-term strategic pivot but may require renewed focus on diversifying product offerings or bundling models.

# Chapter 2: Profitability Trends

Despite macroeconomic headwinds, Microsoft maintained healthy profitability:
	•	Gross margin improved to $34.7B, a 9.5% increase indicating strong cost control.
	•	Operating income rose 6.3%, reflecting disciplined spending across R&D and administrative channels.
	•	However, net income dropped by 14.4%, largely due to a sharp increase in income tax provisions. Q1 FY2023 saw a $4.02B tax charge, compared to just $19M in Q1 FY2022.

Insight: While core operations remain profitable, tax volatility poses short-term pressure on bottom-line performance.

# Chapter 3: Operational Efficiency

Microsoft’s key performance indicators reflect overall resilience but reveal areas for optimization:

   KPI                           Formula                            Q1FY2023        Q1FY2022         
   Gross Margin %                Gross MArgine/Revenue              69.2%           69.9%            
   Operating Margin %            Operating Income/Revenue           42.9%           44.6%
   Net Margin %                  Net Income/Revenue                 35%             45.3%

   The decline in margins, particularly Net Margin, underscores the outsized impact of tax and expense volatility.

# Chapter 4: Variance Breakdown

A variance waterfall chart was constructed to illustrate how each cost and revenue line item contributed to total change in operating income. Notable increases were seen in:
	•	R&D Spend (+18.4%)
	•	Sales and Marketing (+12.7%)
	•	Service and Other Cost (+13.1%)

Meanwhile, product revenue and net income showed negative variance, triggering alerts for further review.

Insight: Cost increases appear investment-driven rather than efficiency losses — suggesting strategic growth spending rather than leakage.

# Chapter 5: Tools & Visualization Summary

Key insights were visualized using both Excel and Power BI dashboards:
	•	The Excel dashboard offered static, high-level KPI tracking, variance bars, and side-by-side comparisons.
	•	The Power BI dashboard allowed users to interact via slicers, drill into specific line items, and dynamically compare Q1 2023 vs Q1 2022 across multiple metrics.

Conclusion: Power BI enhanced storytelling and exploration, while Excel offered simplicity for quick insights and traditional reporting formats.

## Files in the Repository

This repository contains the following files to showcase the full scope of the analysis:
📊 Microsoft_PnL_Variance_Analysis.xlsx
Contains the raw data table, variance calculations, KPIs, and the static Excel dashboard.
📈 Microsoft_PnL_Variance_Dashboard.pbix
An interactive Power BI version of the dashboard with slicers, tooltips, and YoY variance comparisons.
📝 README.md
Full project documentation covering the background, methodology, analysis, results, and insights.
