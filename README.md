<img width="150" height="150" align="right" alt="elezaby_en" src="https://github.com/user-attachments/assets/3c1aa919-3edb-41d6-8f3d-accaea3477f9" />

# Elezaby E-commerce Analytics Dashboard

## Project Overview
This project involves a comprehensive analysis of an online pharmacy's sales data. The goal was to transform raw datasets into an interactive Power BI dashboard, providing insights into sales performance, customer behavior, and product associations to drive strategic business decisions.

## Business Tasks
The analysis aimed to:
1.  Clean and prepare raw data for analysis.
2.  Extract key insights across sales, customer behavior, and product performance.
3.  Conduct advanced RFM segmentation to classify customers.
4.  Perform market basket analysis to uncover cross-sell opportunities.
5.  Build an interactive dashboard to present a clear business story.

## Data Sources
The analysis uses three primary datasets:
1.  **orders_fact.csv**: Contains order-level information (`order_id`, `customer_id`, `order_date`).
2.  **order_products_fact.csv**: Contains line-item details for each order (`order_id`, `product_id`, `quantity`, `unit_price`, `sales`).
3.  **products_dimension.csv**: Contains product information (`product_id`, `product_name`, `category`, `subcategory`, `unit_price`).

## Data Model
I built a **Star Schema** data model in Power BI for optimal performance and simplicity:
*   **Fact Tables:** `orders_fact`, `order_products_fact`
*   **Dimension Tables:** `products_dimension`, `Date` (custom created date table)
*   **Relationships:** Established one-to-many relationships between dimension and fact tables.

## Key Metrics & Analysis
### Core KPIs
*   Total Sales, Total Orders, Unique Customers
*   Average Order Value (AOV), Average Items per Order

### Advanced Analysis
1.  **RFM Customer Segmentation:**
    *   Calculated Recency, Frequency, and Monetary value for each customer.
    *   Scored each dimension (1-5) and segmented customers into categories: Champions, Loyal Customers, At Risk, Lost Customers.
2.  **Market Basket Analysis (Association Rules):**
    *   Created a product pairs table to identify frequently bought-together items.
    *   Calculated pair frequency to derive top cross-selling opportunities.

## Dashboard
The interactive Power BI report consists of three pages:

1.  **Executive Summary:** High-level overview of KPIs, monthly sales trends, top products, and basket size distribution.
2.  **Customer Analysis:** Deep dive into RFM segments with a donut chart, detailed table, and sales by segment.
3.  **Product & Basket Analysis:** Features top product pairs and a drill-through product hierarchy matrix. Includes actionable insights and recommendations.

## Tools & Technologies
*   **Power BI:** Data cleaning, data modeling, DAX, visualization, and dashboard design.
*   **Power Query (M):** Used for data transformation and cleaning.

## How to Use
1.  Download the `Elezaby_Analytics.pbix` file.
2.  Open it in Power BI Desktop.
3.  Interact with the slicers and visuals to explore the data. Use the drill-down features in the matrix visual to explore product categories.

## Insights & Recommendations
1.  **Loyalty Program:** A small segment of "Champion" customers drives most revenue. Implement a loyalty program with exclusive offers to retain them.
2.  **Product Bundling:** Top product pairs (e.g., Shampoo & Conditioner) should be bundled and promoted via a "Frequently Bought Together" widget.
3.  **Checkout Optimization:** Since most orders are 1-2 items, implement add-on suggestions at checkout to increase average basket size.

## Project Structure
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

# Author
**Mahmoud Abdallah**
## Any Questions
**Mahmoud_Abdallah20@outlook.com**
