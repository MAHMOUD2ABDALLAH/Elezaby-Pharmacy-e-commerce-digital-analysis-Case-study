# Elezaby Pharmacy Case Study Dashboard

## Project Overview

This project involves a comprehensive analysis of an online pharmacy's sales data. The goal was to transform raw datasets into an interactive Power BI dashboard, providing insights into sales performance, customer behavior, and product associations to drive strategic business decisions.

## Business Tasks

The analysis aimed to:
1. Clean and prepare raw data for analysis.
2. Extract key insights across sales, customer behavior, and product performance.
3. Conduct advanced RFM segmentation to classify customers.
4. Perform market basket analysis to uncover cross-sell opportunities.
5. Build an interactive dashboard to present a clear business story.

---

## Page 1: Executive Summary

<img width="1000" height="580" alt="Elezaby1" src="https://github.com/user-attachments/assets/8cf1bc68-64fe-47a4-9a4c-f0f6322273cf" />

### Key Visuals & Metrics

| Metric | Description |
|--------|-------------|
| Core KPIs | Total Sales, Total Orders, Unique Customers, Average Order Value (AOV), Average Items per Order |
| Monthly Sales Trends | Line chart showing sales over time |
| Top Products | Bar chart of best-selling products by revenue or quantity |
| Basket Size Distribution | Histogram of number of items per order |

---

## Page 2: Customer Analysis

<img width="1000" height="580" alt="Elezaby2" src="https://github.com/user-attachments/assets/6a73ab8b-7397-4a58-970f-e4874819c908" />

### Key Visuals & Metrics

| Analysis | Description |
|----------|-------------|
| RFM Customer Segmentation | Recency, Frequency, Monetary scoring (1–5) |
| Customer Segments | Champions, Loyal Customers, At Risk, Lost Customers (donut chart) |
| Sales by Segment | Bar or column chart showing revenue contribution per segment |
| Customer Detail Table | Interactive table with individual customer RFM scores |

---

## Page 3: Product & Basket Analysis

<img width="1000" height="580" alt="Elezaby3" src="https://github.com/user-attachments/assets/5807271e-bf92-4eca-a9f6-1258eb01defc" />

### Key Visuals & Metrics

| Analysis | Description |
|----------|-------------|
| Top Product Pairs | Frequently bought together items (market basket analysis) |
| Product Hierarchy Matrix | Drill-through matrix by category and subcategory |
| Actionable Insights | Recommendations for bundling and cross-selling |

---

## Data Sources

The analysis uses three primary datasets:

1. **orders_fact.csv** – Order-level information (`order_id`, `customer_id`, `order_date`)
2. **order_products_fact.csv** – Line-item details per order (`order_id`, `product_id`, `quantity`, `unit_price`, `sales`)
3. **products_dimension.csv** – Product master data (`product_id`, `product_name`, `category`, `subcategory`, `unit_price`)

## Data Model

A **Star Schema** was built in Power BI:

- **Fact Tables:** `orders_fact`, `order_products_fact`
- **Dimension Tables:** `products_dimension`, `Date` (custom calendar)
- **Relationships:** One-to-many between dimensions and fact tables

## Key Metrics & Advanced Analysis

### Core KPIs

- Total Sales, Total Orders, Unique Customers
- Average Order Value (AOV), Average Items per Order

### Advanced Analysis

1. **RFM Customer Segmentation** – Recency, Frequency, Monetary scoring (1–5) → segments: Champions, Loyal Customers, At Risk, Lost Customers.
2. **Market Basket Analysis** – Product pairs frequency to identify top cross‑sell opportunities.

## Tools & Technologies

- **Power BI** – Data cleaning, modeling, DAX, visualizations, dashboard design
- **Power Query (M)** – Data transformation and cleaning

## How to Use

1. Download the `Elezaby_Analytics.pbix` file.
2. Open it in Power BI Desktop.
3. Use slicers and visuals to explore. Drill down in the matrix visual to see product categories.

## Insights & Recommendations

1. **Loyalty Program** – A small “Champion” customer segment drives most revenue. Offer exclusive perks to retain them.
2. **Product Bundling** – Top pairs (e.g., Shampoo & Conditioner) should be bundled and promoted via a “Frequently Bought Together” widget.
3. **Checkout Optimization** – Most orders are 1–2 items. Implement add‑on suggestions at checkout to increase basket size.

## Project Structure
```
Elezaby-Ecommerce-Analytics/
│
├── Data/ (optional - add raw CSVs if you can)
│ ├── orders_fact.csv
│ ├── order_products_fact.csv
│ └── products_dimension.csv
│
├── Assets/ (optional - add screenshot of dashboard)
│ └── dashboard_overview.png
│
├── Elezaby_Analytics.pbix
└── README.md
```
# Author
**Mahmoud Abdallah**
## Any Questions
**Mahmoud_Abdallah20@outlook.com**

<img width="200" height="200" alt="Elezaby" src="https://github.com/user-attachments/assets/2bd6a1d4-1b45-4a15-8ac7-dad07a457eaa" />

