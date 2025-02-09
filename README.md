# Sales Data Analysis

## Overview
This project analyzes e-commerce sales data to derive valuable insights, detect trends, and support data-driven decision-making. The dataset includes transaction details such as order dates, product names, purchase addresses, and sales amounts.

## Objectives
- Clean and preprocess the raw sales data
- Perform exploratory data analysis (EDA) to identify key trends and patterns
- Engineer features to improve data quality
- Visualize the insights using Python libraries

## Dataset Description
The dataset contains 12 CSV files containing sales details for the 12 months of the year 2019.
Each file contains anywhere from around 9000 to 26000 rows and 6 columns.
The dataset consists of the following key attributes:
- **Order ID**: Unique identifier for each order
- **Product**: Name of the product purchased
- **Quantity Ordered**: Number of units ordered
- **Price Each**: Price per unit
- **Order Date**: Timestamp of the order
- **Purchase Address**: Shipping address of the customer

## Data Preprocessing Steps

### 1. Handling Missing and Erroneous Data
- Removed rows with missing values
- Filtered out erroneously included header rows
- Converted `Quantity Ordered` and `Price Each` columns to appropriate data types
- Converted the `Order Date` column to a DateTime format, correcting invalid entries

### 2. Removing Duplicates
- Identified and removed 618 duplicate rows to ensure data integrity

### 3. Feature Engineering
- **Total Sales Calculation**: Created a new column `Total` by multiplying `Quantity Ordered` and `Price Each`
- **Date Components**: Extracted day, month, and hour from the `Order Date` for time-based analysis
- **Location Extraction**: Split the `Purchase Address` column to derive City, State, and Zip Code

### 4. Data Sorting and Final Checks
- Sorted the dataset by `Order Date` to maintain chronological order
- Standardized city names to avoid inconsistencies

## Key Insights & Visualizations
Using Python and libraries like Pandas, NumPy, Seaborn, and Matplotlib, key insights were extracted and visualized:
- **Sales Trends**: Identified peak sales months and daily trends
- **Best-Selling Products**: Recognized the most popular items
- **City-wise Sales Distribution**: Analyzed which locations have the highest revenue
- **Hourly Sales Analysis**: Explored customer purchase behaviour throughout the day
- **Frequently Bought Together Products**: Identified product pairings that are frequently bought together

## Tools & Technologies Used
- **Python Libraries**:
  - **Pandas**: For data manipulation and cleaning
  - **NumPy**: For numerical operations and array manipulation
  - **Seaborn**: For data visualization and statistical plotting
  - **Matplotlib**: For creating various static, animated, and interactive plots
  - **OS**: For file management and directory operations
- **Jupyter Notebook**: For interactive data exploration and analysis

## What I Have Done in This Project

This project involves analyzing e-commerce sales data to uncover insights that can support business decision-making. The main tasks performed include data preprocessing, exploratory data analysis (EDA), and generating key business insights.

## Data Processing

Data processing includes cleaning and preparing the data for analysis. The main steps include handling missing or erroneous data, removing duplicates, and creating additional features (such as total sales and date components).

## Exploratory Data Analysis (EDA)

EDA is the key part of the project where we explore the data to uncover valuable insights.

### Sales Analysis

#### Best Month for Sales
We calculate the total sales per month to identify the month with the highest sales.

#### What Day of the Week Has the Highest Sales?
We analyze the data to determine which day of the week has the highest sales.

#### Timeline of Day of the Week vs. Revenue
We visualize sales revenue based on the day of the week to identify patterns.

#### Sales Per Hour
We examine the sales distribution per hour to understand peak purchasing times.

### Product Analysis

#### What Product Sold the Most?
We identify the best-selling product based on the total quantity sold.

#### Top Products for Each City
We determine the top-selling products by city.

#### Top 5 Products with the Highest Revenue for Each City
We identify the top 5 products generating the most revenue in each city.

#### What Products Are Most Often Sold Together?
We analyze product pairings to identify frequently bought-together items.

#### What Percentage of Orders Include Multiple Products?
We calculate the percentage of orders that include more than one product.

### Order Value Analysis

#### What Was the Highest Single-Order Value?
We identify the highest value for a single order.

### City and Revenue Analysis

#### What City Has the Highest Revenue?
We determine the city with the highest total revenue.

#### What City Sold the Most Products?
We identify the city with the highest sales volume.

### State Analysis

#### What Is the Distribution of States?
We analyze the distribution of sales across different states.

## Conclusion

Through this sales data analysis, we derived key insights that can support business decision-making. These insights include peak sales months, the most popular products, top revenue-generating cities, and more. The findings can help optimize business operations, enhance marketing strategies, and maximize revenue. Continuous analysis of sales data is essential for adapting to changing market conditions and maintaining a competitive edge.

