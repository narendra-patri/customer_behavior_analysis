# customer_behavior_analysis
Data Analytics project showcasing customer behavior analysis using python, sql and power bi
🛍️ Customer Shopping Behavior Analysis

Python | SQL (PostgreSQL) | Power BI | Business Insights

🔍 Project Overview

This project analyzes customer shopping behavior across 3,900 transactions to uncover patterns in spending, product preferences, discounts, subscriptions, and customer loyalty.

The objective is to transform raw transactional data into actionable business insights using Python, SQL, and Power BI—mirroring real-world data analyst workflows.

📊 Dataset

Source: Customer Shopping Behavior Dataset (CSV)

Rows: 3,900

Columns: 18

Key Features

Customer Demographics: Age, Gender, Location, Subscription Status

Purchase Details: Item Purchased, Category, Purchase Amount, Season, Size, Color

Behavioral Metrics:

Discount Applied

Promo Code Usage

Previous Purchases

Frequency of Purchases

Review Rating

Shipping Type

Data Quality Notes

37 missing values in review_rating

Resolved using category-level median imputation

🛠️ Tools & Technologies
Programming & Analysis

Python (Pandas, NumPy, Matplotlib, Seaborn)

Jupyter Notebook

Databases & SQL

PostgreSQL

SQL (Aggregations, Joins, Window Functions, Ranking)

Visualization & Reporting

Power BI (Interactive Dashboard)

Analytical Report (PDF)

Business Presentation (Gamma / PPT)

🔄 Project Workflow
1️⃣ Data Loading & Inspection

Loaded raw CSV using Pandas

Verified schema, data types, and summary statistics

2️⃣ Exploratory Data Analysis (EDA)

Distribution analysis of purchase amounts and ratings

Customer behavior trends across gender, age, and category

Identification of outliers and inconsistencies

3️⃣ Data Cleaning & Feature Engineering

Imputed missing review ratings using category medians

Standardized column names to snake_case

Engineered new features:

age_group

purchase_frequency_days

Identified redundancy between discount_applied and promo_code_used

Dropped promo_code_used

4️⃣ SQL Business Analysis (PostgreSQL)

Cleaned data was loaded into PostgreSQL and analyzed using SQL to answer key business questions:

Revenue by gender

High-spending customers who still used discounts

Top 5 products by average review rating

Standard vs Express shipping spend comparison

Subscribers vs non-subscribers revenue

Products most dependent on discounts

Customer segmentation (New / Returning / Loyal)

Top products within each category

Relationship between repeat purchases and subscriptions

Revenue contribution by age group

📂 All queries available in customer_behavior_queries.sql

📈 Power BI Dashboard

An interactive Power BI dashboard was created to visualize insights for stakeholders.

Dashboard Highlights

Gender Revenue Split:

Male customers generate 68% of total revenue

Female customers contribute 32%

Customer Segmentation:

Loyal (5+ purchases): 3,116 customers (~80%)

Returning (2–4 purchases): 701

New (1 purchase): 83

Product Performance:

Gloves → Highest average rating (3.86)

Blouse → Most purchased clothing item

Jewelry → Top-performing accessory category

Subscription Insights:

Only 27% customers are subscribers

Average spend is nearly identical for subscribers vs non-subscribers

📂 Power BI file: customer_behavior.pbix

📌 Key Insights & Results

Male customers generate 2.1× more revenue than female customers

839 customers used discounts but still spent above average

Loyalty is strong, but subscription adoption is relatively low

Express shipping users tend to spend more per transaction

Certain products rely heavily on discounts, impacting margins

💡 Business Recommendations

Boost Subscriptions: Introduce exclusive subscriber-only benefits

Strengthen Loyalty Programs: Reward repeat buyers to retain the dominant loyal segment

Optimize Discount Strategy: Reduce over-discounting on high-demand products

Product Positioning: Promote top-rated and best-selling items

Targeted Marketing: Focus on high-revenue age groups and express shipping users

▶️ How to Run the Project

Clone the repository:

git clone https://github.com/your-username/customer-shopping-behavior-analysis.git


Install required libraries:

pip install pandas numpy matplotlib seaborn psycopg2


Open Jupyter Notebook:

jupyter notebook


Run:

Customer_behavior_project.ipynb

Load cleaned data into PostgreSQL

Execute SQL queries from:

customer_behavior_queries.sql

Open customer_behavior.pbix in Power BI to explore the dashboard
