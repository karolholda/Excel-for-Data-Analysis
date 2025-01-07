# Coffee Shop Sales Analysis 2019 - 2022

![Dashboard Overview](https://github.com/karolholda/Excel-for-Data-Analysis/blob/main/Coffee%20Shop%20Project/assets/csd1.jpg)

## 📊 Project Overview

This project focuses on analyzing sales data for a coffee shop between 2019 and 2022. The goal was to extract actionable insights to better understand customer behavior, optimize product offerings, and improve operational efficiency. The dataset required extensive preprocessing, including handling duplicates, standardizing date formats, and ensuring data integrity for meaningful analysis.

### Key Objectives:
- **Identify the top 5 most loyal customers** their purchasing behavior.
- **Analyze sales distribution by country** to understand regional preferences.
- **Evaluate coffee consumption patter** based on strength, size, and customer preferences.
- **Understand the impact of loyalty cards** based on strength, size, and customer preferences.
- - **Create a dynamic timeline slider** to visualize sales trends over time.

## 📅 Data Overview

![Data Table](https://github.com/karolholda/Excel-for-Data-Analysis/blob/main/Coffee%20Shop%20Project/assets/csd2.jpg)

The dataset included detailed sales transaction data with the following fields:
- **Order Date** Dates of customer purchases, which were standardized for analysis.
- **Product Details** Coffee strength, size, and additional product features.
- **Quantity** Number of items sold per transaction.
- **Transaction Value** Total value of the order.
- **Loyalty Card** Indication of whether a loyalty card was used.
- **Location Data** Country information for regional analysis.

## 🛠 Tools Used

**1. Data Cleaning and Preparation:**

- **Standardized date format**s using TEXT and DATEVALUE functions.
- **Removed duplicate** transactions using Excel's built-in tools.
- **Corrected inconsistencies** in product names and formatted fields for clarity.
  
**2. Formulas and Calculations**

- **Utilized INDEX MATCH and XLOOKUP** to merge and retrieve data efficiently.
- **Applied advanced formulas**, such as SUMIFS and IFERROR, to aggregate data and handle missing values.
- **Used multiplication formulas** to calculate total sales values.
  
**3. Data Transformation**

Converted raw datasets into structured tables.
Designed and formatted tables for clear presentation and analysis.
Built pivot tables to summarize sales data by product, customer, and region.
Visualizations and Dashboard Creation

Designed charts to represent sales trends, product popularity, and customer behavior:
Line Charts: Visualized sales trends over time.
Bar Charts: Displayed revenue by product type and region.
Pie Charts: Illustrated sales by coffee strength and size.
Inserted slicers and a timeline slider to allow for dynamic filtering and analysis.

## 📈 Dashboard Insights

The interactive dashboard provides a detailed breakdown of the sales performance of **Savory Bites**:

- **Monthly Sales Analysis**: Tracks sales trends over time, with the highest sales occurring in July and December.
- **Revenue from Each Product**: Sandwiches and Frankies were the top-performing items, generating the most revenue.
- **Sales by Payment Method**: The majority of transactions were completed using cash (48%), followed by online payments (40%).
- **Sales by Time of Day**: Night-time sales were the highest (23%), indicating the busiest period for the restaurant.
- **Average Order Value**: The highest average order value came from sandwich orders, with other fast food items following closely.

## 🧹 Data Cleaning Story

The original dataset from **Kaggle** was far from perfect and required significant preprocessing before any meaningful analysis could be performed. One of the biggest challenges was dealing with inconsistent and incomplete data:

1. **Date Format Issues**: Dates were provided in multiple formats, which made time-series analysis difficult. Some dates were in "MM/DD/YYYY" format, while others were in "DD-MM-YYYY", and even text representations like "July 23rd". I had to standardize all date formats using Excel’s `DATEVALUE` function to ensure consistency.

2. **Missing Payment Methods**: A large portion of transactions lacked information about the payment method. To resolve this, I analyzed patterns within the existing data. For example, larger transaction amounts were often paid via online payment, so I imputed missing values based on these patterns. I also filled in missing values using the most common payment method for certain time periods and products.

3. **Product Name Inconsistencies**: Product names were entered inconsistently (e.g., "Sugar Cane Juice" vs. "Sugarcane juice"). These inconsistencies were corrected through manual review and the use of `VLOOKUP` to standardize names.

These steps ensured the dataset was reliable for analysis and helped generate more accurate insights into customer behavior and sales performance.

## 🌟 Key Findings

- **Top Products**: Sandwiches and Frankies were the most popular and generated the highest revenue.
- **Payment Method Preferences**: A large percentage of customers preferred to pay with cash, followed by online payments.
- **Peak Hours**: The night period (20:00-23:00) had the highest sales, indicating that this is the busiest time for the restaurant.
- **Seasonality**: Sales peaked in July and December, which could inform future inventory and staffing decisions.
