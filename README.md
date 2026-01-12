# 🛒 E-Commerce Data Analysis
## Online Shopping Trends, Customer Behavior & Sales Performance

---

## 1. Project Overview
This project presents an end-to-end data analysis of an online shopping platform, focusing on understanding customer behavior, sales performance, product trends, payment patterns, and delivery efficiency. The analysis demonstrates how structured business data can be transformed into actionable insights that support strategic decision-making in an e-commerce environment.

The project combines data engineering, exploratory data analysis, and business interpretation to address real-world operational and commercial questions faced by online retailers.

---

## 2. Business Motivation
E-commerce businesses generate large volumes of transactional and operational data. However, without systematic analysis, this data provides limited value.

This project aims to answer key business questions such as:
- How do customers behave and spend over time?
- Which products and suppliers drive the most revenue?
- How effective are delivery and fulfillment processes?
- How do reviews and ratings influence sales?

Insights from this analysis can inform marketing strategies, inventory planning, supplier management, and logistics optimization.

---

## 3. Data Source
The dataset was sourced from Kaggle and represents a simulated online shopping platform.

It consists of **eight relational datasets**:
- Customers
- Orders
- Order Items
- Products
- Payments
- Reviews
- Shipments
- Suppliers

Each dataset captures a different aspect of the e-commerce pipeline, allowing for a holistic analysis of customer journeys and business operations.

> **Note:** Raw data files are not included in this repository due to size and licensing constraints. The full data schema and processing steps are documented in the notebook.

---

## 4. Database Design
A relational database was created using **SQLite** to organize and manage the data efficiently.

Key design principles:
- Primary keys for unique identification
- Foreign keys to enforce relationships
- Referential integrity across all tables
- Scalable structure suitable for business growth

An Entity–Relationship Diagram (ERD) was created to visualize table relationships and guide database construction.

---

## 5. Data Preprocessing & Feature Engineering
Significant preprocessing was required to prepare the data for analysis:

### Data Cleaning
- Conversion of date fields to datetime format
- Removal of duplicate records
- Detection of outliers using the Interquartile Range (IQR) method

### Data Integration
- Merging multiple tables to create a unified analytical dataset
- Linking customers to orders, payments, products, reviews, and shipments

### Feature Engineering
Derived features include:
- Customer Lifetime Value (CLV)
- Total revenue by product and category
- Order frequency and order size
- Review counts and average ratings
- Delivery performance indicators (on-time vs delayed)

These features enabled deeper behavioral and performance analysis.

---

## 6. Exploratory Data Analysis
Exploratory analysis focused on identifying patterns and trends across the business:

- Sales and order volume trends over time
- Customer spending distributions and repeat purchase behavior
- Product and supplier revenue contributions
- Relationship between reviews, ratings, and purchase volume
- Delivery efficiency across carriers and time periods

Visualizations were used extensively to support interpretation and communication.

---

## 7. Key Insights
- Approximately **70% of orders contain 1–3 items**, indicating preference for smaller purchases
- **Top 10 customers contribute ~25% of total revenue**, highlighting the importance of retention
- Sales peak during festive periods but decline afterward
- Certain products and suppliers consistently outperform others
- Delivery delays negatively impact customer satisfaction and trust

---

## 8. Business Recommendations
Based on the analysis, the following recommendations are proposed:
- Implement targeted marketing campaigns during low-demand periods
- Introduce loyalty programs for high-value customers
- Optimize inventory for top-performing products
- Monitor supplier quality and delivery reliability
- Encourage customer reviews through automated follow-ups and incentives

---

## 9. Limitations
- Dataset represents a single simulated platform
- No predictive or machine learning models were applied
- External market and economic factors not included

---

## 10. Conclusion
This project demonstrates how structured data analysis can uncover meaningful insights across customer behavior, sales trends, and operational efficiency in an e-commerce setting. By integrating multiple data sources and focusing on business-relevant metrics, the analysis highlights opportunities for revenue growth, improved customer satisfaction, and operational optimization.

---

## 11. Repository Structure
```text
notebooks/        → Jupyter notebook with full analysis  
reports/          → Detailed project report  
images/           → Visual outputs used in this README  
data/raw/         → Raw data source description  
data/processed/   → Processed data description  
