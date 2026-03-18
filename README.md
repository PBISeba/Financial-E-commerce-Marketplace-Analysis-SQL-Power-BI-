# Financial-E-commerce-Marketplace-Analysis-SQL-Power-BI-
 End-to-end business intelligence project combining SQL data transformation and Power BI analytics. The project focuses on financial performance, customer structure, and product category dynamics in a Brazilian e-commerce marketplace.

## Project Overview

This project combines SQL-based data preparation with Power BI data modeling and visualization.

Data was pre-aggregated and transformed using SQL (PostgreSQL), then modeled and analyzed in Power BI using DAX measures and interactive visuals.

The dashboard focuses on:

• Financial performance and revenue trends  
• Customer structure and revenue concentration  
• Product category performance and demand patterns  

## Dashboard Preview

![Dashboard Overview](screenshots/financial_performance.png)

## SQL Data Preparation

Part of the data transformation logic was implemented in SQL before loading into Power BI.

Key SQL components:

• Aggregated monthly revenue (aggregate_monthly_sales)  
• Top customers ranking (aggregate_top_customers)  
• Data cleaning and transformation logic  
• Pre-calculated metrics to improve performance  

This approach reduces model complexity in Power BI and improves report performance.

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


## Technical Stack

Power BI  
DAX  
SQL (PostgreSQL)  
Data Modeling (Star Schema)  
Power Query  
Interactive dashboard design






