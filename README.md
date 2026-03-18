# Financial E-commerce Marketplace Analysis (SQL + Power BI)

End-to-end business intelligence project combining SQL data transformation and Power BI analytics.

Designed as a portfolio-ready BI solution demonstrating a full analytics workflow — from data preparation to interactive dashboarding.

The project focuses on financial performance, customer structure, and product category dynamics in a Brazilian e-commerce marketplace.

---

## Project Overview

This project combines SQL-based data preparation with Power BI data modeling and visualization.

Data was pre-aggregated and transformed using SQL (PostgreSQL), then modeled and analyzed in Power BI using DAX measures and interactive visuals.

The dashboard focuses on:

• Financial performance and revenue trends  
• Customer structure and revenue concentration  
• Product category performance and demand patterns  

---

## Dashboard Preview

![Dashboard Preview](screenshots/Intro.png)
![Dashboard Preview](screenshots/Financial_Performance.png)
![Dashboard Preview](screenshots/Customer_Structure_and_Concentration.png)
![Dashboard Preview](screenshots/Product_Analysis.png)
---

## SQL Data Preparation

Part of the data transformation logic was implemented in SQL before loading into Power BI.

Key SQL components:

• Aggregated monthly revenue (aggregate_monthly_sales)  
• Top customers ranking (aggregate_top_customers)  
• Data cleaning and transformation logic  
• Pre-calculated metrics to improve performance  

This approach reduces model complexity, improves performance, and separates transformation logic from the reporting layer.

---

## Dataset

The dataset represents a Brazilian e-commerce marketplace (Olist-style transactional dataset) and includes:

• Orders and transaction data  
• Customer information and geographic location  
• Product categories  
• Revenue metrics  

Time range: **2016–2018**  
Currency: **BRL with dynamic USD conversion**

The dataset structure follows a **star schema data model** optimized for analytical queries.

---

## Data Model

The report uses a star schema model with SQL-based pre-aggregations.

Fact table:

• fact_sales – transactional order data  

Dimensions:

• dim_calendar  
• dim_customer  
• dim_product_category  
• dim_rates (currency conversion)

Additional helper tables were implemented for dynamic report features (Top-N, currency switch, filters).

![Data Model](screenshots/Data_Model.png)

---

## Key Features

• Dynamic currency switch (BRL / USD)  
• Top-N analysis with automatic "Others" grouping  
• Pareto analysis for revenue concentration  
• Interactive filter panel (time, geography, product)  
• KPI overview for financial and operational metrics  
• Cross-filtering across all visuals  
• Separation of SQL and DAX logic for performance and scalability  

---

## Dashboard Pages

### Financial Performance
Analysis of revenue trends, growth dynamics, and overall marketplace performance.

Key insights:
• Revenue trends over time  
• Year-over-year growth  
• Revenue distribution across product categories  

---

### Customer Structure & Concentration
Analysis of customer distribution and revenue concentration across regions.

Key insights:
• Pareto analysis of revenue by state  
• Customer distribution across key regions  
• ARPU comparison across top states  

---

### Product Analysis
Evaluation of product category performance and demand patterns.

Key insights:
• Revenue vs order volume by category  
• Product category revenue distribution  
• Average revenue per customer by category  

---

### SQL vs DAX (Work in Progress)


---

## Technical Stack

Power BI  
DAX  
SQL (PostgreSQL)  
Data Modeling (Star Schema)  
Power Query  
Interactive dashboard design  
