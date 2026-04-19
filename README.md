# Financial KPI Monitoring & Profitability Dashboard

## Objective
Build a Power BI dashboard to monitor core financial KPIs, compare budget vs actual performance, and analyze profitability across regions, departments, product categories, customer segments, and sales channels.

## Tools Used
- Power BI Desktop
- Power Query
- DAX
- Excel / CSV
- GitHub
- LinkedIn

## Dataset Description
The sample dataset contains 120 rows and 20 columns:
- Date, Month, Quarter, Year
- Region, Department
- Product Category, Product Name
- Revenue, Cost of Goods Sold, Operating Expenses
- Gross Profit, Net Profit, Profit Margin %
- Sales Volume
- Budgeted Revenue, Actual Revenue, Budget Variance
- Customer Segment, Sales Channel

## Recommended Power Query Steps
1. Import the CSV/XLSX file into Power BI.
2. Check column data types.
3. Remove nulls and duplicates.
4. Standardize text values for Region, Department, Category, and Channel.
5. Create or validate Month, Quarter, and Year fields from Date.
6. Format financial fields as Currency and Profit Margin as Percentage.

## Suggested DAX Measures
```DAX
Total Revenue = SUM('FinancialData'[Revenue])

Total Cost = SUM('FinancialData'[Cost of Goods Sold]) + SUM('FinancialData'[Operating Expenses])

Gross Profit = SUM('FinancialData'[Gross Profit])

Net Profit = SUM('FinancialData'[Net Profit])

Profit Margin % = DIVIDE([Net Profit], [Total Revenue], 0)

Budgeted Revenue = SUM('FinancialData'[Budgeted Revenue])

Actual Revenue = SUM('FinancialData'[Actual Revenue])

Budget Variance = [Actual Revenue] - [Budgeted Revenue]
```

## Dashboard Features
- KPI cards for Revenue, Gross Profit, Net Profit, Profit Margin %, Budget Variance
- Revenue by Region
- Profit by Product Category
- Monthly Revenue and Profit Trend
- Sales Channel Distribution
- Revenue to Net Profit Waterfall
- Matrix table by Region
- Slicers for Region, Department, Product Category, Sales Channel, Month

## Key Insights
- Identify top-performing regions and product categories
- Compare actual revenue against budget
- Monitor margin movement over time
- Track cost pressure and channel-wise profitability
- Support leadership decision-making with one-page reporting

## Screenshots
Create a `screenshots/` folder and add:
- dashboard-overview.png
- kpi-cards.png
- regional-revenue-chart.png

Embed them in the README using:
```md
![Dashboard Overview](screenshots/dashboard-overview.png)
```

## Conclusion
This project is a strong portfolio case for Finance Analyst, FP&A Analyst, Business Analyst, and MBA students because it demonstrates data cleaning, modeling, DAX, KPI design, business storytelling, and professional presentation.
