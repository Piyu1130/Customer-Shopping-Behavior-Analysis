🛍️ **Customer Shopping Behavior Analysis**
📌 Project Overview

This project analyzes customer shopping behavior using transactional data from 3,900 purchases across multiple product categories.
The objective is to uncover insights related to customer demographics, spending patterns, product preferences, discounts, subscriptions, and purchase frequency to support data-driven business decisions.

The analysis combines Python (EDA & data cleaning), SQL (business queries), and Power BI (dashboard visualization).

📊 **Dataset Summary**

Total Records: 3,900
Total Columns: 18

**Key Features**
Customer Demographics:
Age
Gender
Location
Subscription Status
Purchase Details:
Item Purchased
Product Category
Purchase Amount
Season
Size
Color
Shopping Behavior:
Discount Applied
Promo Code Used
Previous Purchases
Purchase Frequency
Review Rating
Shipping Type

**Missing Values:**

37 missing entries in the Review Rating column

🧹 **Exploratory Data Analysis (Python)**

EDA and preprocessing were performed using Python (Pandas, NumPy).

**Key Steps**

Data loading and inspection (df.info(), df.describe())

**Handling missing values:**

Imputed missing Review Ratings using median rating per product category

**Column standardization:**

Converted column names to snake_case

**Feature engineering:**

Created age_group feature by binning ages

Derived purchase_frequency_days

**Data validation:**

Identified redundancy between discount_applied and promo_code_used

Dropped promo_code_used

**Database integration:**

Loaded cleaned data into PostgreSQL for SQL-based analysis

🗄️ Data Analysis using SQL (PostgreSQL)

Business-focused SQL queries were executed to extract actionable insights.

**Key Analyses**

Revenue comparison by gender

Identification of high-spending customers using discounts

Top 5 products by average review rating

Average purchase comparison by shipping type

Subscribers vs Non-Subscribers spending analysis

Products most dependent on discounts

**Customer segmentation:**

New

Returning

Loyal

Top 3 products within each category

Relationship between repeat purchases and subscription status

Revenue contribution by age group

📈 Power BI Dashboard

An interactive Power BI dashboard was created to visualize insights such as:

Revenue trends

Customer segmentation

Product performance

Subscription impact

Discount behavior

The dashboard enables stakeholders to explore insights dynamically and supports strategic decision-making.

💡 Business Recommendations

Increase Subscriptions:
Offer exclusive deals and benefits to convert repeat customers into subscribers.

Customer Loyalty Programs:
Incentivize returning customers to move them into the “Loyal” segment.

Optimize Discount Strategy:
Control margin erosion while maintaining sales volume.

Product Positioning:
Highlight top-rated and best-selling products in marketing campaigns.

Targeted Marketing:
Focus campaigns on high-revenue age groups and express-shipping users.

🛠️ Tools & Technologies Used

Python: Pandas, NumPy

Database: PostgreSQL

Visualization: Power BI

IDE: Jupyter Notebook

Version Control: Git & GitHub

📂 Project Structure
Customer-Shopping-Behavior-Analysis/
│
├── data/
│   └── raw_dataset.csv
│
├── notebooks/
│   └── customer_behavior_eda.ipynb
│
├── sql/
│   └── business_analysis_queries.sql
│
├── dashboard/
│   └── power_bi_dashboard.pbix
│
├── README.md

