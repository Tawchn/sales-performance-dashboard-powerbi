# sales-performance-dashboard-powerbi
A simple, clean Power BI project that demonstrates a star schema model and core DAX measures to analyse sales performance across customers, products, and time.

This dashboard answers:
- How much did we sell (revenue)?
- Which products and categories drive the most sales?
- Which customers, cities, and segments contribute the most?
- How do sales change over time?

[dashbord overall view](overview.png)
## Dataset
This project uses a small sample dataset (CSV) created for learning and demonstration.

Tables:
- Customers (dimension)
- Products (dimension)
- Sales (fact)

Files are included in the `data/` folder.

## Data Model (Star Schema)
Relationships:
- Customers[CustomerID] → Sales[CustomerID] (1:* )
- Products[ProductID] → Sales[ProductID] (1:* )



## Measures (DAX)
Create these measures in Power BI:

## DAX
Total Sales = SUM(Sales[SalesAmount])

Total Quantity = SUM(Sales[Quantity])

Average Sale = AVERAGE(Sales[SalesAmount])

