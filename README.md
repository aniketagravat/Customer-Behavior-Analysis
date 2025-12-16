# Customer Shopping Behavior Analysis

## Overview
This project analyzes customer purchasing behavior using transactional retail data to identify revenue drivers, customer segments, and the impact of discounts and subscriptions on spending. The analysis follows an end-to-end analytics workflow using Python, SQL (PostgreSQL), and Power BI.

The goal is not visualization for the sake of charts, but actionable business insights.

---

## Dataset
- **Records:** 3,900 customer purchases  
- **Features:** 18 columns  
- **Data Includes:**
  - Customer demographics (age, gender, location, subscription status)
  - Purchase details (category, item, amount, season, size, color)
  - Shopping behavior (discount usage, purchase frequency, reviews, shipping type)

Missing values were found only in the `review_rating` column and handled systematically.

---

## Tools & Technologies
- **Python:** pandas, numpy (data cleaning & feature engineering)
- **SQL:** PostgreSQL (business analysis queries)
- **BI Tool:** Power BI (interactive dashboard)
- **Database:** PostgreSQL
- **Version Control:** Git & GitHub

---

## Data Preparation (Python)
- Loaded and explored raw data using pandas
- Standardized column names to snake_case
- Handled missing review ratings using **median imputation by product category**
- Engineered new features:
  - `age_group`
  - `purchase_frequency_days`
- Identified and removed redundant features (`promo_code_used`)
- Loaded the cleaned dataset into PostgreSQL for SQL-based analysis

---

## SQL Analysis (Business Questions Answered)
The following business questions were answered using PostgreSQL:

1. Revenue contribution by gender  
2. High-spending customers who still used discounts  
3. Top 5 products by average review rating  
4. Purchase amount comparison by shipping type  
5. Subscriber vs non-subscriber spending behavior  
6. Products most dependent on discounts  
7. Customer segmentation (New, Returning, Loyal)  
8. Top 3 products per category  
9. Relationship between repeat purchases and subscriptions  
10. Revenue contribution by age group  

All queries were written with a business-first approach, not just technical complexity.

---

## Power BI Dashboard
An interactive dashboard was built to visualize:
- Revenue trends
- Customer segmentation
- Subscription impact
- Shipping preferences
- Product performance

The dashboard enables non-technical stakeholders to explore insights without SQL or Python knowledge.

---

## Key Insights
- Subscribers generate higher average revenue than non-subscribers
- Loyal customers contribute disproportionately to total revenue
- Certain products rely heavily on discounts, impacting margins
- Express shipping users tend to spend more per purchase
- Specific age groups dominate revenue contribution

---

## Business Recommendations
- Strengthen subscription incentives to increase customer lifetime value
- Introduce loyalty programs to convert repeat buyers into loyal customers
- Re-evaluate discount strategies for margin-heavy products
- Focus marketing efforts on high-performing products and revenue-driving age groups

---

## Project Structure
