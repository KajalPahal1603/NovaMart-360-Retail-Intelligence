NovaMart 360 — Retail Intelligence Dashboard

Power BI | DAX | Data Modeling | Retail Analytics

Project Overview

NovaMart 360 is an interactive Power BI retail analytics project designed to analyze sales performance, customer purchasing behavior, and product profitability.

The dashboard uses a synthetic retail dataset and includes three analytical report pages.

Dashboard Preview

1. Sales Overview

[Sales Overview](Sales_Overview.png)

2. Customer Analysis

[Customer Analysis](Customer_Analysis.png)

3. Product Performance

[Product Performance](Product_Performance.png)

Key Features

- Sales, profit, orders, and profit margin KPIs
- Monthly sales trends and year-over-year comparisons
- Regional and category-level sales analysis
- Actual sales vs. sales targets
- Customer segmentation and repeat purchase analysis
- Customer lifetime sales analysis
- Top customers by revenue and order frequency
- Product sales, profitability, and profit margin rankings
- Interactive Power BI visualizations and filters

Key Metrics

| Metric | Value |
|---|---|
| Total Sales | £1.32M |
| Total Profit | £569.30K |
| Profit Margin | 43.05% |
| Total Customers | 356 |
| Repeat Customers | 336 |
| Repeat Customer Rate | 94.38% |
| Products Sold | 30 |
| Sales Target Achievement | 13.64% |

*Metrics represent the report's unfiltered overview and may change with filters.*

Tools and Technologies

- Microsoft Power BI Desktop
- DAX (Data Analysis Expressions)
- Power Query
- Excel
- GitHub

Data Model

The project uses the following tables:

- Orders
- Products
- Customers
- Stores
- Calendar
- Returns
- TargetsData

Sample DAX Measures

Total Sales

dax
Total_Sales =
SUMX(
    Orders,
    Orders[Quantity] * Orders[PricePerUnit]
)


Repeat Customer Rate**

```dax
Repeat Customer Rate =
DIVIDE(
    [Repeat Customers],
    [Total Customers],
    0
)
```

**Average Orders per Customer**

```dax
Average Orders per Customer =
DIVIDE(
    [Total Orders],
    [Total Customers],
    0
)
```

Project Files

- Power BI `.pbix` file — interactive report
- Excel `.xlsx` file — synthetic retail dataset
- Dashboard screenshots — previews of all three pages

How to Use

1. Download the Power BI `.pbix` file.
2. Open it in Microsoft Power BI Desktop.
3. Explore the three report pages.
4. Use available slicers and visual interactions to analyze the data.

Created as a data analytics portfolio project to demonstrate Power BI reporting, DAX calculations, data modeling, and retail business analysis.
