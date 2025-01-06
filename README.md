# 🛒 Fill That Cart! Analyzing Customer Behavior on Instacart 🛍️
## 📖 Project Overview
This project explores customer purchasing behaviors on the Instacart platform by analyzing a dataset containing detailed order and product information. The goal was to uncover trends in shopping patterns, popular products, and customer loyalty. The analysis was structured into three main steps: data description, preprocessing, and advanced exploration.

## 🛠 Step-by-Step Implementation
### 1. Data Description
Objective
Understand the structure and quality of the data before diving into preprocessing and analysis.

Process
Loaded five datasets: instacart_orders.csv, products.csv, aisles.csv, departments.csv, and order_products.csv.
Examined the data with methods such as info(), head(), and describe() to identify data types, missing values, and duplicates.
Key Findings
Orders: Some rows contained duplicate entries, and missing values were present in the days_since_prior_order column.
Products: Missing product names were identified, all tied to a specific department and aisle.
Order Products: Missing values in add_to_cart_order and no major issues with duplicates.
Aisles and Departments: Clean data without duplicates or missing values.
### 2. Data Preprocessing
Objective
Prepare the datasets for analysis by resolving data quality issues.

Steps Taken
Corrected Data Types: Ensured all ID columns were integers.
Handled Missing Values:
Replaced missing product_name with "Unknown."
Imputed missing add_to_cart_order values with 999 and converted to integers.
Removed Duplicates:
Dropped duplicate rows in the orders and products datasets.
Insights
Addressing missing and duplicate values ensured clean and reliable data for further analysis.
### 3. Data Analysis
A. Easy-Level Insights
Order Times:
Most orders occurred between 10 a.m. and 4 p.m., peaking around noon.
Shopping was most frequent on Sundays and Mondays.
Reorder Frequency:
Average time between orders was ~11 days, with a median of 7 days.
B. Intermediate-Level Insights
Daily Trends:
Shopping patterns on Wednesdays and Saturdays were similar, with peaks around mid-morning.
Orders per Customer:
Most customers placed between 1 and 5 orders, with a few outliers exceeding 20 orders.
Top Products:
Popular items included chocolate sandwich cookies, organic bananas, and avocados.
C. Advanced-Level Insights
Cart Size:
The average order contained ~10 items.
Reordered Products:
Chocolate sandwich cookies and organic bananas were frequently reordered, indicating high customer loyalty.
First Items Added to Cart:
Items like milk, bananas, and avocados were commonly the first to be added to carts.
Reorder Ratios:
Certain products showed a 100% reorder ratio, indicating consistent customer preference.
## 📊 Visualizations
Hourly and Daily Trends: Bar charts showcasing order frequency by time and day.
Reorder Behavior: Histograms and bar plots highlighting customer loyalty patterns.
Product Popularity: Top 20 reordered products visualized for better insights.
## 🧠 Conclusions
Customer Behavior:
Customers frequently shop on Sundays and Wednesdays, adding ~10 items per order.
Many customers show loyalty by repeatedly ordering the same products.
Product Popularity:
Staples like bananas, milk, and avocados are among the most frequently purchased items.
Business Opportunities:
Insights into customer preferences can guide personalized marketing and product placement strategies.
