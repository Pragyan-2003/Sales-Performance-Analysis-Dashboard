# Sales Performance Analysis Dashboard

## Project Overview
This project focuses on analyzing sales performance using Power BI.  
The dashboard provides valuable insights into revenue, profit, customer behavior, product performance, and regional sales trends to support business decision-making.

---

## Objectives
- Monitor overall sales performance
- Analyze profit and revenue trends
- Identify top-performing products and customers
- Compare regional sales performance
- Track monthly and yearly growth

---

## Tools & Technologies Used
- Power BI
- Power Query
- DAX
- CSV

---

## Dataset Files
- sales.csv
- customers.csv
- products.csv
- dates.csv

---

## Key KPIs
- Total Revenue
- Total Profit
- Total Orders
- Profit Margin
- Average Revenue Per Customer
- Monthly Sales Growth

---

## Dashboard Features

### Sales Analysis
- Monthly and yearly revenue trends
- Running total revenue analysis
- Sales growth tracking

### Product Analysis
- Top-selling products
- Category-wise sales performance
- Product profit contribution

### Customer Analysis
- Revenue by customer
- Top customers by sales
- Customer purchasing patterns

### Regional Analysis
- Region-wise revenue and profit
- Geographic sales comparison

---

## DAX Measures Used

### Total Revenue
```DAX
Total Revenue = SUM(Sales[Revenue])
```

### Total Profit
```DAX
Total Profit = SUM(Sales[Profit])
```

### Profit Margin
```DAX
Profit Margin = DIVIDE([Total Profit],[Total Revenue],0)
```

### Average Revenue Per Customer
```DAX
Avg Revenue Per Customer =
DIVIDE([Total Revenue], DISTINCTCOUNT(Customers[CustomerID]))
```

---

## Key Insights
- Technology category generated the highest revenue.
- Western region contributed maximum sales.
- Seasonal sales spikes observed during festival periods.
- High-value customers contributed a significant share of total revenue.

---

## Conclusion
This dashboard helps businesses track sales trends, monitor profitability, identify growth opportunities, and make data-driven business decisions effectively.

---
