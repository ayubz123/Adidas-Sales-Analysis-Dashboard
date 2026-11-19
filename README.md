# Adidas Sales Analysis Dashboard (2020--2021)

## Project Overview

This project analyzes Adidas US sales data for 2020--2021 using
Microsoft Excel, focusing on sales performance, operating profitability,
retailer and regional comparisons, and sales-channel trends.

## Business Objectives

-   Evaluate sales and operating profit across retailers and regions.
-   Compare operating margins and sales methods.
-   Examine weekly and annual sales trends.
-   Identify business patterns that may require further investigation.

## Dataset

Adidas US Sales dataset (2020--2021), including retailer, location,
product, invoice date, sales method, units sold, total sales, operating
profit, and operating margin. A day-of-week field was derived from the
invoice date.

## Tools & Techniques

Microsoft Excel, Power Query, PivotTables, PivotCharts, formulas, KPI
cards, and slicers.

## Data Cleaning & Preparation

-   Removed two invalid records labelled `zero` in the Retailer field:
    one summary-like record and one mostly-zero record without a valid
    transaction.
-   Converted invoice dates using locale-aware settings.
-   Created a day-of-week field from the invoice date.
-   Renamed and reordered fields.
-   Prepared approximately 9,949 cleaned records.

## Dashboard Structure
!(1-Overall%20Overview.png)
1.  Overall Overview
2.  Detailed Analysis
3.  Key Insights
4.  Outlet Performance & Trends

Interactive slicers: Year, Month, Sales Method, Retailer, Product, and
Region. Slicers are connected across relevant dashboard views.

## Key Performance Indicators
!(2-Detailed%20%Analysis.png)

-   Total Sales: sum of sales.
-   Operating Profit: sum of operating profit.
-   Units Sold: total units sold.
-   Operating Margin: total operating profit divided by total sales.

## Key Business Insights
!(3-Key%20Insights.png)

### 1. Weekly Sales Performance

Thursday and Friday record the highest total sales and the highest
average sales. Monday has the lowest total sales, while Saturday has the
lowest average sales. Keep total and average performance distinct.

### 2. Retailer Sales & Profitability

The retailer with the highest sales is not necessarily the retailer with
the highest operating margin. Assess retailers using sales, operating
profit, and margin together---not sales volume alone.

### 3. Regional Sales & Profitability

The West region generates the highest sales but has an operating margin
of approximately 33%. The South records the highest operating margin at
approximately 42%. Higher sales do not automatically translate into
stronger profitability.

### 4. Retailer Margin Comparison

West Gear generates approximately \$243 million in sales with an
operating margin of about 35%. Sport Direct generates approximately
\$182.5 million with a margin of about 41%, while Walmart records
approximately \$74.6 million in sales and a margin of about 35%.

### 5. Annual Sales Growth (2020 vs. 2021)

Total sales are substantially higher in 2021 than in 2020. Further
breakdown by sales method, region, and product can identify where the
increase occurred; the comparison alone does not establish its causes.

### 6. West Region -- Outlet Channel Performance

In the West region, In-store and Outlet each generate approximately
\$105 million in sales. In-store contributes 39% of the region's total
operating profit, compared with 36% from Outlet. Outlet sales decline
steadily during the second half. These percentages are shares of
regional operating profit, not channel margins.

### 7. Regional Outlet Performance in 2021

Outlet performance varies across regions during 2021. The Northern
region shows increases in Q2 and Q4, while other regional trends
generally show declines. Review Outlet performance by region rather than
treating it as one uniform pattern.

### 8. Outlet Performance by Retailer in 2021
!(4-Outlet%20Performance%20&%20Trends.png)

West Gear records approximately \$24.8 million in Outlet sales in Q1,
compared with approximately \$1.5 million across Q2--Q4 combined. Kohl's
records approximately \$40.5 million in the first half, followed by
approximately \$0.3 million in the second half. These sharp differences
warrant validation and closer investigation.

## Business Recommendations

-   Review pricing, discounting, product mix, and operating costs where
    high sales are not matched by stronger margins.
-   Investigate the second-half Outlet decline in the West region.
-   Examine sharp retailer-level quarterly fluctuations.
-   Use regional, retailer, and sales-method filters to locate
    performance changes.
-   Treat possible causes as hypotheses unless supported by additional
    operational data.

## Conclusion

Sales volume alone is not enough to evaluate business performance.
Combining sales, operating profit, and operating margin provides a more
balanced view, while regional, retailer, channel, and weekly analysis
reveals patterns hidden in overall totals.

## Repository Structure

``` text
Adidas Sales Analysis Dashboard (2020-2021)/
├── Adidas Sales Analysis.xlsx
├── Dashboard Screenshots/
│   ├── Overall Overview.png
│   ├── Detailed Analysis.png
│   ├── Key Insights.png
│   └── Outlet Performance & Trends.png
├── Adidas_Sales_Analysis_Insights_Report.pdf
└── README.md
```

*Approximate figures are rounded. Findings describe patterns in the
dataset and do not prove their underlying causes.*
