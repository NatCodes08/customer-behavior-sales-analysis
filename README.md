# Customer Behaviour and Sales Performance Analysis

## Project Overview
This project analyses retail transaction data to understand customer purchasing behaviour, sales performance, product trends and customer segmentation.

Using Python, SQL and data visualization techniques, the project explores transactional data to identify meaningful business insights and support data-driven decision-making.

![Sales and Customer Dashboard](reports/retail_dashboard.png)

## Business Objectives
- Analyse overall sales performance and monthly revenue trends.
- Identify top-performing products based on revenue and quantity sold.
- Understand customer purchasing patterns and repeat purchases.
- Identify high-value customers and customers at risk of becoming inactive.
- Segment customers using RFM (Recency, Frequency, Monetary) analysis.
- Generate actionable business recommendations.

## Tools and Technologies
- Python
- Pandas and NumPy
- Matplotlib
- SQL
- SQLite
- Google Colab
- Microsoft Excel
- GitHub

## Dataset
The project uses the Online Retail dataset from the UCI Machine Learning Repository.

The dataset contains retail transaction records from December 2010 to December 2011.

Initial dataset size: 541,909 records.

## Project Workflow

### 1. Data Exploration
- Examined dataset structure, dimensions and data types.
- Identified missing values and duplicate records.
- Investigated cancelled transactions and negative quantities.
- Examined unusual and zero unit prices.

### 2. Data Cleaning
- Removed cancelled transactions.
- Removed records with non-positive quantities and unit prices.
- Removed missing customer IDs and product descriptions.
- Removed duplicate records.

Final cleaned dataset: 392,692 records.

### 3. Feature Engineering
Created additional columns:
- TotalSales
- Year
- Month
- MonthName
- Date

### 4. Exploratory Data Analysis
Analysed:
- Monthly sales performance.
- Product-wise revenue and quantity sold.
- Customer spending and purchase frequency.
- Sales distribution across countries.

### 5. Customer Segmentation
Applied RFM analysis using:
- Recency: Time since the customer's last purchase.
- Frequency: Number of distinct orders.
- Monetary: Total customer spending.

Customers were classified into four segments:
- Best Customers
- Loyal Customers
- Potential Customers
- At Risk Customers

### 6. SQL Analysis
Used SQLite to store and analyse transaction and customer segmentation data.

SQL queries were used to identify:
- Top-performing products.
- Revenue by country.
- Monthly revenue trends.
- Customer segment distribution.

## Key Findings

| Metric | Result |
|---|---:|
| Total cleaned records | 392,692 |
| Total revenue | 8,887,208.89 |
| Unique customers | 4,338 |
| Unique products | 3,665 |
| Unique invoices | 18,532 |
| Repeat customer rate | 65.58% |

### Additional Insights
- November 2011 recorded the highest monthly revenue.
- PAPER CRAFT, LITTLE BIRDIE was the highest-revenue product.
- The United Kingdom generated the highest revenue.
- 1,295 customers were classified as At Risk Customers.
- 1,260 customers were classified as Best Customers.

## Business Recommendations
- Develop targeted re-engagement campaigns for at-risk customers.
- Introduce personalized offers to encourage repeat purchases.
- Focus on retaining high-value customers through exclusive benefits.
- Monitor monthly sales trends to improve inventory and promotional planning.
- Evaluate international markets to identify opportunities for business growth.

## Project Structure

```text
Customer_Behaviour_Sales_Analysis/
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
├── sql/
├── reports/
└── README.md
```

## Conclusion
This project demonstrates how retail transaction data can be transformed into meaningful business insights using Python, SQL and data visualization. It highlights customer purchasing patterns, product performance, sales trends and customer segments that can support better business decisions.