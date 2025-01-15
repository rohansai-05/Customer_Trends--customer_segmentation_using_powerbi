# Customer Segmentation Analysis using Power BI

This project analyzes customer shopping trends using Power BI to identify distinct customer segments based on purchasing behavior, demographics, and preferences. These insights help businesses tailor marketing strategies, enhance customer engagement, and optimize resource allocation.

## Project Overview

- **Objective**: 
  - Identify customer segments based on their unique characteristics.
  - Optimize marketing efforts by targeting segments with tailored strategies.
  - Enhance resource allocation by focusing on valuable customer groups.

- **Data Source**: Kaggle (Customer shopping trends dataset)

- **Scope of Analysis**: 
  - Customer demographics
  - Purchase history
  - Product categories
  - Order values and other metrics

## Data Preprocessing

1. **Data Cleaning**:
   - Address missing values.
   - Handle duplicates.
   - Correct inconsistencies.

2. **Data Transformation**:
   - Restructure data by splitting columns and merging tables.
   - Create calculated fields for analysis.

3. **Data Type Corrections**:
   - Ensure consistency (e.g., dates as Date, numbers as Decimal).

4. **Calculated Columns and Measures**:
   - Use DAX (Data Analysis Expressions) for advanced analysis and visualization.

## DAX Measures

Key DAX calculations used in the project:

- **Total Sales**: `SUM(Sales[Amount])`
- **Total Profit**: `SUM(Sales[Profit])`
- **Average Price per Unit**: `AVERAGE(Sales[PricePerUnit])`
- **Yearly Profit**: `CALCULATE(SUM(Sales[Profit]), Sales[Year])`
- **Sales by Category**: `CALCULATE(SUM(Sales[Amount]), Sales[Category])`
- **Profit Margin**: `DIVIDE(SUM(Sales[Profit]), SUM(Sales[Amount]))`
- **Units Sold by Region**: `CALCULATE(SUM(Sales[Units]), Sales[Region])`

## Key Insights

1. **Demographics**:
   - Customers aged 40–60 years contribute the most to purchases.
   - Male customers dominate the customer base.

2. **Sales Trends**:
   - Highest sales for clothing in Spring.
   - Strong accessory sales in Fall.

3. **Shipping and Payment**:
   - Free shipping is the most preferred option.
   - Credit card is the dominant payment method.

4. **Seasonal Patterns**:
   - Winter exhibits the highest purchase frequency.

## Tools and Technologies

- **Power BI**: For data visualization and insights.
- **DAX**: For creating measures and calculated columns.
- **Power Query**: For advanced data manipulation.

## How to Run the Project

1. Download the dataset from Kaggle.
2. Load the dataset into Power BI.
3. Perform data preprocessing using Power Query.
4. Use the provided DAX measures to create visualizations.
5. Explore insights and derive actionable conclusions.


