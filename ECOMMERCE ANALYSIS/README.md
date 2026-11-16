# E-Commerce Sales Analysis Dashboard (Power BI)

An interactive Power BI dashboard that analyses 5,000 e-commerce orders across revenue, categories, regions, payment methods, customers, ratings and delivery performance.


## Project Overview

The goal of this project is to turn raw order data into a clear, filterable view of business performance, so that sales trends, top segments and operational gaps can be spotted quickly.

## Key Metrics

| Metric | Value |
|---|---|
| Total Revenue | ₹51,09,776 |
| Total Orders | 5,000 |
| Total Customers | 989 |
| Total Quantity Sold | 20,224 |
| Average Order Value | ~₹1,022 |

## Dashboard Visuals

- **KPI cards:** Total Revenue, Orders, Customers, Quantity Sold
- **Revenue by Category:** column chart
- **Revenue by Payment Method:** donut chart (Card, COD, Wallet)
- **Revenue by Region:** bar chart
- **Monthly Revenue Trend:** line chart (Jan to Dec)
- **Top 10 Customers by Revenue:** bar chart by Customer ID
- **Average Customer Rating by Category**
- **Average Delivery Days by Region**
- **Slicers:** Order Date, Region, Payment Method, Product Category

## Key Insights

- **Electronics** is the top category at about 36% of revenue (₹18.30L), followed by Clothing (~30%), Home (~19%) and Beauty (~15%).
- **West** is the top region (₹13.46L); the four regions are close, ranging from ₹12.36L to ₹13.46L.
- **Payment mix:** Card is the largest share (~46%), followed by COD (35%) and Wallet (~19%).
- **Seasonality:** revenue peaks in May (₹4.80L) and is lowest in April (₹3.99L).
- **Customer quality:** ratings are almost flat across categories (2.94 to 3.01 out of 5), indicating room to improve satisfaction.
- **Delivery:** average delivery time is about 6.1 days with little variation between regions (6.08 to 6.17 days).
- **Customer 1663** is the highest-value customer (about ₹17,681).

## Tools and Skills Used

- Power BI Desktop
- Data cleaning (Excel)
- DAX measures and calculated columns (e.g. `Month Short`, `Month Number`)
- Data modelling and sorting by column
- Dashboard design: layout, formatting, slicers, consistent colour theme

## Repository Structure

```
├── Ecommerce_Cleaned_Data.xls        # Cleaned dataset
├── Ecommerce_Analysis.pbix           # Power BI report file
├── Ecommerce_Analysis_Dashboard.pdf  # Exported dashboard
├── Dashboard_Preview.png             # Dashboard screenshot
└── README.md
```

## How to Use

1. Clone or download this repository.
2. Open `Ecommerce_Analysis.pbix` in Power BI Desktop.
3. If prompted, point the data source to `Ecommerce_Cleaned_Data.xls`.
4. Use the slicers on the left to filter by date, region, payment method and category.

## Possible Improvements

- Add Average Order Value and Average Rating KPI cards
- Add repeat-customer rate and late-delivery % analysis
- Highlight the top category and region with a darker colour
- Add page navigation for the sidebar buttons
