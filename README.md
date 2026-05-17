# Sales Performance Analysis Dashboard

## Overview
The Sales Performance Analysis Dashboard is an interactive Power BI project designed to analyze and visualize business sales data.  
This dashboard helps in monitoring revenue, profit, customer trends, product performance, and regional sales insights to support data-driven decision-making.

---

## Project Objectives
- Analyze overall sales performance
- Monitor revenue and profit trends
- Identify top-performing products and customers
- Compare sales across different regions
- Track business growth over time
- Generate actionable business insights

---

## Tools & Technologies
- Power BI
- Power Query
- DAX (Data Analysis Expressions)
- CSV

---

## Dataset Information
The project uses multiple datasets for data modeling and analysis:

| Dataset | Description |
|---|---|
| sales.csv | Contains transaction-level sales data |
| customers.csv | Customer-related information |
| products.csv | Product and category details |
| dates.csv | Date dimension table for time analysis |

---

## Data Cleaning & Transformation
The following preprocessing steps were performed using Power Query:

- Removed duplicate records
- Handled missing/null values
- Corrected data types
- Standardized column names
- Created relationships between tables
- Performed date formatting
- Cleaned inconsistent category values

---

## Data Model
The dashboard follows a relational data model using:
- Fact Table: Sales
- Dimension Tables:
  - Customers
  - Products
  - Dates

Relationships were created to enable efficient filtering and analysis.

---

## Key Performance Indicators (KPIs)
The dashboard tracks the following KPIs:

- Total Revenue
- Total Profit
- Total Orders
- Profit Margin
- Average Revenue Per Customer
- Monthly Sales Growth
- Running Total Revenue

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
Profit Margin =
DIVIDE([Total Profit], [Total Revenue], 0)
```

### Average Revenue Per Customer
```DAX
Avg Revenue Per Customer =
DIVIDE(
    [Total Revenue],
    DISTINCTCOUNT(Customers[CustomerID])
)
```

---

## Dashboard Features

### Sales Analysis
- Revenue trend analysis
- Monthly and yearly sales comparison
- Running total revenue tracking

### Product Analysis
- Top-selling products
- Category-wise sales performance
- Profit contribution by product category

### Customer Analysis
- Top customers by revenue
- Customer purchase behavior
- Revenue contribution analysis

### Regional Analysis
- Region-wise revenue comparison
- Profit analysis by region
- Geographic sales distribution

---

## Key Insights
- Technology products generated the highest revenue.
- Western region contributed the maximum sales.
- Seasonal spikes were observed during festive months.
- A small percentage of customers contributed a major share of total revenue.
- Certain product categories showed high sales but low profit margins.

---

## Business Impact
This dashboard enables businesses to:
- Monitor sales performance effectively
- Identify profitable products and regions
- Improve customer targeting strategies
- Support strategic business decisions
- Track growth and operational efficiency

---

## Conclusion
The Sales Performance Analysis Dashboard provides a comprehensive view of business performance through interactive visualizations and KPI tracking.  
The project demonstrates skills in data cleaning, data modeling, DAX calculations, and dashboard design using Power BI.

