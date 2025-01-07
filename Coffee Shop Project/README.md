# Coffee Shop Sales Analysis 2019 - 2022

![Dashboard Overview](https://github.com/karolholda/Excel-for-Data-Analysis/blob/main/Coffee%20Shop%20Project/assets/csd1.jpg)

## 📊 Project Overview

This project focuses on analyzing sales data for a coffee shop between 2019 and 2022. The goal was to extract actionable insights to better understand customer behavior, optimize product offerings, and improve operational efficiency. The dataset required extensive preprocessing, including handling duplicates, standardizing date formats, and ensuring data integrity for meaningful analysis.

### Key Objectives:
- **Identify the top 5 most loyal customers** their purchasing behavior.
- **Analyze sales distribution by country** to understand regional preferences.

## 📅 Data Overview

![Data Table](https://github.com/karolholda/Excel-for-Data-Analysis/blob/main/Coffee%20Shop%20Project/assets/csd2.jpg)

The dataset consists of detailed records of sales transactions, including:
- **Order Date**: The date on which the order was placed, but this field contained multiple formatting errors that had to be corrected.
- **Item Name**: The specific product purchased.
- **Item Type**: Categorizes items into "Fastfood" or "Beverages".
- **Quantity**: Number of items purchased in a transaction.
- **Transaction Amount**: The total cost of the transaction.
- **Transaction Type**: The method of payment (Cash, Online, Other). This column had numerous missing or unclear values, requiring manual review and imputation.
- **Received By**: Whether the transaction was handled by Mr. or Mrs.
- **Time of Sale**: Categorized into Morning, Afternoon, Evening, Night, or Midnight.

## 🛠 Tools Used

- **Microsoft Excel**: Used for data cleaning, preprocessing, and analysis.
  - **Data Cleaning**: The dataset required extensive cleaning, especially in the date and transaction type columns:
    - **Date Issues**: Dates were entered in multiple formats, making it difficult to perform time-based analysis. I used Excel’s `TEXT` and `DATEVALUE` functions to standardize all date formats.
    - **Missing Payment Methods**: Many rows lacked transaction type information (Cash, Online, Other). I applied a combination of `IF` and `VLOOKUP` functions to fill in missing values based on patterns in the data, such as assuming "Online" for large orders or filling missing values based on the frequency of similar transactions.
    - **Duplicates and Inconsistencies**: The data had duplicate entries, which were removed using Excel’s `REMOVE DUPLICATES` tool, and inconsistencies in product names that were corrected with `VLOOKUP` and manual review.
  - **Advanced Functions**: Formulas such as `SUMIFS`, `VLOOKUP`, and `IFERROR` were used to aggregate and correct data.
- **Pivot Tables**: Employed to summarize sales data by product, time of sale, and transaction type.
- **Charts and Visualizations**: A variety of charts were used to visualize sales trends, product popularity, and customer behavior:
  - **Line Charts**: For monthly sales analysis.
  - **Bar Charts**: To display revenue per product and the number of items sold.
  - **Pie Charts**: To show sales distribution by payment method and time of day.

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
