# Target Brazil E-Commerce Business Case Analysis

## 📊 Project Overview

This is a comprehensive **data-driven business case analysis** of Target's Brazil e-commerce operations (2016–2018). The project demonstrates end-to-end analytics capabilities including SQL query optimization, data exploration, trend analysis, and strategic business recommendations.

**Completed as part of the Scaler Data Science & Machine Learning Course – Business Analytics Module**

---

## 🎯 Objective

Analyze Target Brazil's 100,000+ order dataset across 8 tables to:
- Understand business growth trajectory and market dynamics
- Identify operational bottlenecks (logistics, payments, delivery)
- Quantify regional performance gaps and opportunities
- Deliver actionable insights and strategic recommendations

**Key Deliverable:** Professional PDF report with 25–30 SQL queries, results, and business analysis.

---

## 📁 Dataset Overview

**Tables Used:**
| Table | Records | Purpose |
|-------|---------|---------|
| `orders` | 100,000+ | Order transactions, timestamps, delivery tracking |
| `customers` | 100,000+ | Customer demographics, state location |
| `order_items` | 300,000+ | Product details, pricing per order |
| `products` | 32,000+ | Product categories, descriptions |
| `payments` | 100,000+ | Payment type, value, installments |
| `order_reviews` | 100,000+ | Review scores, customer satisfaction |
| `sellers` | 3,000+ | Seller info, location, performance |
| `product_category_translation` | Lookup | Category name mappings |

**Data Period:** September 2016 – October 2018  
**Platform:** Google BigQuery (Standard SQL)

---

## 📊 Analysis Sections

### **Section 1: Initial Exploration (15 pts)**
- Data types, time range, geographic coverage
- 3 foundational queries

### **Section 2: In-Depth Exploration (15 pts)**
- Yearly trends, seasonality, time-of-day patterns
- 3 queries with visual insights

### **Section 3: E-Commerce Evolution (10 pts)**
- Growth by state, customer distribution evolution
- 2 strategic queries

### **Section 4: Impact on Economy (20 pts)** ⭐
- Revenue growth YoY (+137%), order pricing analysis
- Freight cost by state
- 3 high-impact queries

### **Section 5: Sales, Freight & Delivery (20 pts)** ⭐
- Delivery time by state (fastest: SP 8 days, slowest: RR 29 days)
- Freight cost analysis (SP R$15/order vs RR R$43/order)
- States exceeding/missing delivery SLAs
- 6 operational queries

### **Section 6: Payment Analysis (10 pts)**
- Payment type distribution (credit card 75%, UPI 19%)
- Installment trends (2–3 installments boost AOV by 35–50%)
- 3 payment queries

### **Section 7: Additional Insights (Bonus)**
- Order status distribution (97% delivered)
- Customer lifetime value by state (SP R$6M, 54% of total)
- Seller performance by state (1,849 sellers in SP vs 4–6 in remote states)
- 4 supplementary queries

**Total: 25–30 SQL Queries | 100 Points**

---

## 🔑 Key Findings

### **Growth & Scale**
- **Orders:** 329 (2016) → 45,101 (2017) → 54,011 (2018)
- **Revenue:** +137% YoY growth (2017→2018)
- **Seasonal Peak:** November–December (5,800–7,500 orders/month)

### **Geographic Concentration**
- **SP dominates:** 42% of customers, 42% of orders, 54% of revenue (R$6M CLV)
- **Top 4 states:** 70% of all revenue (SP, RJ, MG, RS)
- **Opportunity:** North/Northeast only 15% of revenue but growing faster

### **Logistics Efficiency Gap**
- **Major states (SP/RJ/MG):** 8–15 day delivery, R$15–21 freight/order (13–18% of price)
- **Remote states (RR/AP/AM):** 23–29 day delivery, R$39–43 freight/order (23–28% of price)
- **Profitability Risk:** 2–3x freight cost in remote regions erodes margins

### **Payment Ecosystem**
- **Credit card:** 75% of orders, highest AOV (R$163)
- **UPI:** 19% of orders, growing 7x (200→1,500 monthly)
- **2–3 Installments:** Boost AOV by 35–50% vs upfront (R$127–143 vs R$94)
- **Vouchers/Debit:** <4% combined, low ROI

### **Delivery Excellence**
- **97% delivery success rate** (96,478 of 99,339 orders delivered)
- **Conservative SLAs:** Remote states deliver 16–20 days EARLY
- **In-transit:** Only 1.1% of orders in "shipped" status (fast turnover)

### **Seller & Product Strategy**
- **SP ecosystem:** 1,849 sellers, 4.01 avg rating, 53,390 5-star orders
- **Tier-2 cities:** PR (349 sellers, 4.07 rating), MG (244 sellers, 4.11 rating)
- **Niche risk:** Small states have <10 sellers, high average prices (R$200–450)

---

## 💡 Actionable Recommendations

### **Immediate (0–3 months)**

1. **Optimize Freight Economics**
   - Implement tiered pricing: minimum order thresholds or surcharges in North/Northeast
   - Free shipping for orders >R$200 to incentivise larger baskets
   - Target: Reduce North/Northeast freight from 23–28% to 18–20% of order price

2. **Payment Channel Focus**
   - Simplify checkout for credit card + UPI (remove vouchers)
   - Launch 2–3 installment plan campaigns
   - Target: Increase AOV by 15–20% (R$94 → R$110)

3. **Q4 Capacity Planning**
   - Build inventory surge: +50% for Q4 (Nov–Dec peaks at 6,000–7,500 orders/month)
   - Expand last-mile capacity: partner with local couriers early

### **Strategic (3–12 months)**

4. **Regional Hub Strategy**
   - Establish distribution centers in **PE, BA, CE**
   - Goal: Reduce North/Northeast delivery from 23+ days to <15 days
   - Unlock R$1–2M additional annual revenue with improved margins

5. **Seller Recruitment & Quality**
   - Recruit 200+ high-quality sellers in **PR, MG, BA** (tier-2 cities)
   - Implement seller SLAs: minimum 3.9 avg rating, <0.5% cancellation
   - Reduce SP dependency: from 56% to 45% of sellers within 18 months

6. **Delivery SLA Optimization**
   - Tighten estimates in major states: SP 8 days, RJ/MG 12 days
   - Leverage conservative remote SLAs: reset to realistic timelines
   - Marketing benefit: "Consistently deliver early" as competitive advantage

7. **Customer Loyalty**
   - Build repeat-purchase program for SP (54% of CLV, need to defend)
   - Premium segment targeting in smaller states (PE/CE/PA with higher per-capita spend)

---

## 🛠️ Technical Stack

| Component | Technology |
|-----------|-----------|
| **Database** | Google BigQuery (Standard SQL) |
| **Data Volume** | 100,000+ orders, 8 tables, 2.5+ years |
| **Query Optimization** | CTEs, window functions, partitioning |
| **Analysis Tool** | Google Sheets / BigQuery UI |
| **Report Format** | Professional PDF (25–30 pages, 100 points) |
| **Languages** | SQL (BigQuery), Markdown |

---

## 📊 SQL Query Patterns Used

✅ **Aggregation & Grouping**
```sql
count(distinct), sum(), avg(), round()
group by, having, order by
```

✅ **Time-Series Analysis**
```sql
extract(year/month/day), 
timestamp_diff(), 
format_timestamp()
```

✅ **Window Functions**
```sql
lag(), lead(), 
partition by, order by
```

✅ **Joins**
```sql
inner join, left join
on o.order_id = p.order_id
```

✅ **Subqueries & CTEs**
```sql
with cte_name as (...)
select ... from cte_name
```

---

## 📈 Key Metrics Summary

| Metric | Value | Insight |
|--------|-------|---------|
| **Total Orders (2016–2018)** | 99,339 | Rapid scaling from pilot to scale |
| **YoY Revenue Growth** | +137% | Doubling in revenue year-over-year |
| **Delivery Success Rate** | 97% | Excellent operational excellence |
| **Average Delivery Time** | 8–15 days (major states) | Competitive vs regional average |
| **Geographic Concentration** | 70% revenue from 4 states | Risk; opportunity in expansion |
| **Freight Cost Variance** | 2.8x (SP vs Remote) | Major profitability gap |
| **Credit Card Dominance** | 75% of orders | Payment method concentration |
| **Customer CLV** | R$144 avg (SP), R$200+ (remote) | Regional pricing power |
| **Seller Concentration** | 56% of sellers in SP | Supply chain risk |

---

## 🚀 How to Use This Repository

### **For Learning:**
1. Review the SQL queries in `/queries/` folder
2. Understand the business logic in each section
3. Replicate queries in your own BigQuery project
4. Modify for different datasets/time periods

### **For Portfolio:**
1. Showcase all 25–30 queries as proof of SQL mastery
2. Highlight business insights beyond just code
3. Demonstrate ability to translate data → decisions
4. Reference in interviews as "end-to-end analytics case"

### **For Hiring Managers:**
- **SQL Skills:** Complex queries, window functions, CTEs
- **Analytics:** 7 business sections, 100+ data points analyzed
- **Business Sense:** Actionable recommendations with ROI quantification
- **Communication:** Professional report, clear insights, strategic thinking

---

## 📁 Repository Structure

```
target-brazil-ecommerce-analysis/
├── README.md (this file)
├── Target-Business-Case-v2.pdf (final deliverable)
├── queries/
│   ├── 1_initial_exploration.sql
│   ├── 2_in_depth_exploration.sql
│   ├── 3_ecommerce_evolution.sql
│   ├── 4_impact_on_economy.sql
│   ├── 5_delivery_analysis.sql
│   ├── 6_payment_analysis.sql
│   └── 7_additional_insights.sql
├── data/
│   ├── query_results/ (CSV exports)
│   └── dataset_schema.md
├── analysis/
│   ├── findings_summary.md
│   ├── recommendations.md
│   └── key_metrics.xlsx
└── images/
    └── dashboard_screenshots/ (query result visualizations)
```

---

## 🎓 Course & Certification

**Program:** Scaler Data Science & Machine Learning Course  
**Module:** Business Analytics / Case Study  
**Task:** End-to-End Data Analysis & Insights Delivery  
**Completion Date:** December 28, 2025  
**Status:** ✅ Submitted & Completed (100/100 points)

---

## 📝 Learning Outcomes

✅ Master BigQuery SQL for large-scale datasets  
✅ Design complex queries with CTEs and window functions  
✅ Translate raw data into business-ready insights  
✅ Identify operational gaps and growth opportunities  
✅ Build professional analytics reports  
✅ Think strategically about e-commerce metrics  
✅ Communicate technical findings to non-technical stakeholders  

---

## 🤝 Contributing

This is a completed case study. For discussions or questions:
- Open an Issue for clarifications
- Submit Pull Requests for improved queries or analysis
- Share portfolio use cases

---

## 📄 License

This project is part of the Scaler Academy Data Science Course curriculum. Use for learning and portfolio purposes only.

---

## 👤 Author

**Your Name**  
Data Science & Analytics Professional  
📧 [Your Email]  
🔗 [Your LinkedIn]  
💼 [Your Portfolio]

---

## ⭐ If you found this helpful, please star this repository!

This comprehensive analysis demonstrates:
- **SQL mastery** with 25–30 production-ready queries
- **Business acumen** with actionable strategic recommendations
- **Communication skills** with clear, executive-level insights
- **Data storytelling** connecting metrics to business impact

**Perfect for:** Portfolio building, interview preparation, real-world analytics practice.

---

**Last Updated:** December 29, 2025  
**Status:** Complete & Production-Ready ✅
