# Sales Performance Dashboard | Microsoft Excel

## Project Overview
End-to-end sales analytics project built on a 9,800-row Global Superstore 
retail dataset spanning 2015–2018 across 4 regions, 3 product categories, 
and multiple customer segments.

## Objective
To simulate a real-world analyst workflow — from raw data validation to 
executive-level dashboard delivery — demonstrating the full data analysis 
lifecycle in Excel.

## Workflow

### Phase 1 — Data Quality & Validation
- Identified 7,301 order-line duplicates and confirmed expected multi-product 
  order structure (not data errors)
- Validated zero blank values across all key columns
- Confirmed date integrity and correct numeric data types across all fields
- Engineered 4 derived columns: Discount, Profit, Month, Quarter — 
  built using business logic where discounts exceeding 20% trigger 
  negative profit, reflecting real retail margin erosion

### Phase 2 — Analysis Layer
Built 20+ formula-driven KPIs using SUMIF, AVERAGEIF, COUNTIF, 
INDEX-MATCH and array formulas:
- Total Revenue, Profit, Orders, Average Discount
- Regional revenue breakdown (West, East, Central, South)
- Category-level revenue and profit comparison
- Average discount analysis by category
- Top customer identification using INDEX-MATCH

### Phase 3 — Pivot Table Analysis
- 4 interconnected pivot tables covering regional performance, 
  category profitability, cross-tabulation (Region × Category), 
  and monthly trend analysis
- Region and Category slicers connected to all pivot tables simultaneously
- One-click filtering updates all tables in real time

### Phase 4 — Executive Dashboard
- KPI banner: Total Revenue, Total Profit, Total Orders, Avg Discount
- Revenue by Region — Column chart
- Revenue by Category — Pie chart  
- Monthly Sales Trend 2015–2018 — Dual-line chart (Sales + Profit)
- Interactive slicers for real-time filtering by Region and Category

## Key Business Insights
- West region led revenue at 31% of total
- Technology category had highest revenue but lowest profit — 
  indicating underlying cost structure inefficiency despite 
  identical discounting across all categories (avg 12%)
- Consistent year-over-year revenue growth with December spikes 
  confirming strong seasonal retail demand patterns
- Top customer by single order value: Sean Miller

## Tools & Techniques
- Microsoft Excel — Tables, Structured References, Named Ranges
- Functions: SUMIF, SUMIFS, AVERAGEIF, COUNTIF, COUNTIFS, 
  INDEX-MATCH, TEXT, CHOOSE, COUNTA, array formulas
- Pivot Tables, Pivot Charts, Slicers
- Dashboard design — KPI cards, multi-chart layout, 
  interactive filtering

## Dataset
Global Superstore Sales Dataset — 9,800 rows, 21 columns  
Source: Kaggle (Rohit Sahoo)  
Period: 2015–2018

## Future Enhancements
- Connect to live data source using Power Query for automated refresh
- Add YoY (Year-over-Year) growth % calculation per region and category
- Build a Salesperson Performance tracker with target vs actual comparison
- Integrate What-If Analysis for discount impact simulation on profit margins
- Migrate dashboard to Power BI for web-based sharing and drill-through capability
- Add a Returns Analysis section tracking return rate by category and region
- Build dynamic Top N customers filter using LARGE and INDEX functions
