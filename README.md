# Target Brazil E-Commerce Business Case Analysis

## Project Overview

Comprehensive data-driven analysis of Target Brazil's e-commerce operations (2016 \- 2018\) with 100,000+ orders across 8 tables.

Key Findings  
Growth Metrics:

- Orders: 329 (2016) to 54,011 (2018)  
- Revenue Growth: \+137% YoY  
- Peak Season: November \- December (6,000+ orders/month)

Geographic Analysis:

- São Paulo (SP) \= 42% of revenue  
- Top 4 states \= 70% of total revenue  
- North/ Northeast \= growth opportunity (15% revenue)

Operational Insights:

- 97% delivery success rate  
- 8-15 day delivery (major states)  
- 23-29 day delivery (remote states)  
- 2-3x freight cost gap between regions

Payment Trends:

- Credit Card: 75% of orders, R$163 avg  
- UPI: 19% of orders, 7x growth YoY  
- Installments: 2-3 months boost AOV 35-50%

Strategic Recommendations

1. Build Regional Hubs in PE/BA/CE to reduce delivery time & freight costs  
2. Tiered Freight Pricing \- increase minimum order value in remote states  
3. Payment Optimization \- focus on credit card \+ UPI only  
4. Seller Recruitment \- 200+ sellers in tier-2 cities (PR, MG, BA)  
5. Delivery SLA Reset \- tighten estimates in major cities, leverage remote efficiency

Projected Impact: R$1-2M additional annual revenue

## Technical Details

Database: Google BigQuery (Standard SQL)  
Analysis: 25-30 SQL queries with CTEs, window functions, complex joins  
Report: PDF

## Dataset

8 tables analyzed: orders (100K+), customers, order\_items (300K+), products, payments, reviews, sellers (3K+), product\_category\_translation  
