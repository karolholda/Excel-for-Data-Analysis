# Coffee Shop Sales Analysis 2019 - 2022

![Dashboard Overview](https://github.com/karolholda/Excel-for-Data-Analysis/blob/main/Coffee%20Shop%20Project/assets/csd1.jpg)

## 📊 Project Overview

This project focuses on analyzing sales data for a coffee shop between 2019 and 2022. The goal was to extract actionable insights to better understand customer behavior, optimize product offerings, and improve operational efficiency. The dataset required extensive preprocessing, including handling duplicates, standardizing date formats, and ensuring data integrity for meaningful analysis.

### Key Objectives:
- **Identify the top 5 most loyal customers** their purchasing behavior.
- **Analyze sales distribution by country** to understand regional preferences.
- **Evaluate coffee consumption patter** based on strength, size, and customer preferences.
- **Understand the impact of loyalty cards** based on strength, size, and customer preferences.
- **Create a dynamic timeline slider** to visualize sales trends over time.

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

- **Converted raw datasets** into structured tables.
- **Designed and formatted tables** for clear presentation and analysis.
- **Built pivot tables** to summarize sales data by product, customer, and region.
  
**Visualizations and Dashboard Creation**

- **Designed charts** to represent sales trends, product popularity, and customer behavior:
- **Line Charts** Visualized sales trends over time.
- **Bar Charts** Displayed revenue by product type and region.
- **Pie Charts** Illustrated sales by coffee strength and size.

**Inserted slicers and a timeline slider to allow for dynamic filtering and analysis.**
------------------------------------------------
## 📈 Dashboard Insights

The final dashboard provided the following insights:

1. **Top Customers**: Identified the top 5 most frequent and high-spending customers, enabling targeted loyalty initiatives.
2. **Regional Sales**: Highlighted country-level sales distribution for regional strategy optimization.
3. **Coffee Preferences**: Showed trends in coffee strength and size preferences, helping refine product offerings.
4. **Loyalty Program Impact**: Demonstrated a 15% higher average spend among loyalty card users.
5. **Sales Trends**: Enabled time-based analysis with an interactive timeline slider.

## 🧹 Data Cleaning Story

The dataset required extensive cleaning to ensure accuracy and usability. Here’s how I approached the challenges:

1. **Date Formatting Issues**  
   - Dates were provided in inconsistent formats (`MM/DD/YYYY`, `DD-MM-YYYY`, and text like "July 23rd"). 
   - Used Excel’s `DATEVALUE` and `TEXT` functions to standardize all dates to a single format, making them usable for time-series analysis.

2. **Duplicates and Inconsistencies**  
   - Detected and removed duplicate entries using Excel’s `Remove Duplicates` feature.
   - Corrected product name inconsistencies (e.g., "Large Coffee" vs. "Coffee Large") using a combination of `VLOOKUP` and manual review.

3. **Missing Values in Payment Method**  
   - Many transactions had missing payment type information. 
   - Filled missing values using logical patterns, such as assuming "Online" for large transactions and imputing the most frequent payment method for smaller ones.

4. **Data Validation**  
   - Applied data validation rules to ensure all future entries adhered to consistent formats, particularly for product names and payment methods.

## 🌟 Key Findings

- **Popular Products**: Strong and medium-strength coffees in larger sizes were the most purchased.
- **Regional Trends**: Sales peaked in countries with colder climates, indicating seasonal consumption patterns.
- **Loyalty Success**: Customers with loyalty cards showed increased purchasing frequency and higher average spend.
- **Seasonality**: December and July consistently had the highest sales, suggesting opportunities for targeted promotions.
- **Dynamic Insights**: The timeline slider revealed clear growth patterns and peak periods.
