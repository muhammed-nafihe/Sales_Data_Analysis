# Sales Data Analysis

## Overview
This project analyses e-commerce sales data to extract meaningful insights, identify trends, and perform data-driven decision-making. The dataset contains transaction details, including order dates, product names, purchase addresses, and sales amounts.

## Objectives
- Clean and preprocess the raw sales dataset
- Perform exploratory data analysis (EDA) to identify trends
- Conduct feature engineering to enhance data quality
- Visualize key insights using Tableau

## Dataset Description
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
- Filtered out header rows mistakenly included in the dataset
- Converted `Quantity Ordered` and `Price Each` columns to appropriate data types
- Converted `Order Date` column to datetime format, handling invalid values

### 2. Removing Duplicates
- Identified and removed 618 duplicate rows to ensure data integrity

### 3. Feature Engineering
- **Total Sales Calculation**: Created a new column `Total` by multiplying `Quantity Ordered` and `Price Each`
- **Date Components**: Extracted day, month, and hour from `Order Date` for time-based analysis
- **Location Extraction**: Split `Purchase Address` to derive City, State, and Zip Code

### 4. Data Sorting and Final Checks
- Sorted the dataset by `Order Date` to maintain chronological order
- Standardized city names to avoid inconsistencies

## Key Insights & Visualizations
The cleaned dataset was analyzed using Tableau to extract insights such as:
- **Sales Trends**: Identifying peak sales months and daily trends
- **Best-Selling Products**: Recognizing the most popular items
- **City-wise Sales Distribution**: Determining which locations have the highest revenue
- **Hourly Sales Analysis**: Understanding customer purchase behavior throughout the day
- **Frequently Bought Together Products**: Identifying common product pairings

## Tools & Technologies Used
- Python (Pandas, NumPy, Matplotlib, Seaborn) for data cleaning and analysis
- Tableau for visualization and dashboard creation
- Jupyter Notebook for interactive data exploration

## Table of Contents
- [Getting Started](#getting-started)
  - [Importing Necessary Libraries](#importing-necessary-libraries)
  - [Loading Data](#loading-data)
  - [Data Processing](#data-processing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
  - [Sales Analysis](#sales-analysis)
    - [Best Month for Sales](#best-month-for-sales)
    - [What Day of the Week Has the Highest Sales?](#what-day-of-the-week-has-the-highest-sales)
    - [Timeline of Day of the Week vs. Revenue](#timeline-of-day-of-the-week-vs-revenue)
    - [Sales Per Hour](#sales-per-hour)
  - [Product Analysis](#product-analysis)
    - [What Product Sold the Most?](#what-product-sold-the-most)
    - [Top Products for Each City](#top-products-for-each-city)
    - [Top 5 Products with the Highest Revenue for Each City](#top-5-products-with-the-highest-revenue-for-each-city)
    - [What Products Are Most Often Sold Together?](#what-products-are-most-often-sold-together)
    - [What Percentage of Orders Include Multiple Products?](#what-percentage-of-orders-include-multiple-products)
  - [Order Value Analysis](#order-value-analysis)
    - [What Was the Highest Single-Order Value?](#what-was-the-highest-single-order-value)
  - [City and Revenue Analysis](#city-and-revenue-analysis)
    - [What City Has the Highest Revenue?](#what-city-has-the-highest-revenue)
    - [What City Sold the Most Products?](#what-city-sold-the-most-products)
  - [State Analysis](#state-analysis)
    - [What Is the Distribution of States?](#what-is-the-distribution-of-states)

## Getting Started

### Importing Necessary Libraries
In this section, we import the required Python libraries to perform data analysis and visualization.

### Loading Data
Data loading is a crucial step in any data analysis project. Here, we load the dataset that we'll be working with. The dataset contains 12 CSV files containing sales details for the 12 months of the year 2019. Each file contains anywhere from around 9000 to 26000 rows and 6 columns. The columns are as follows:
- Order ID
- Product
- Quantity Ordered
- Price Each
- Order Date
- Purchase Address

### Data Processing
Data processing involves cleaning and preparing the data for analysis. This section includes various data preprocessing steps.

## Exploratory Data Analysis (EDA)

EDA is the heart of this project, where we explore and analyze the data to gain insights.

### Sales Analysis

#### Best Month for Sales
We determine the best month for sales and present our findings.

#### What Day of the Week Has the Highest Sales?
We identify the day of the week with the highest sales and provide insights.

#### Timeline of Day of the Week vs. Revenue
We visualize the timeline of day of the week versus revenue to spot trends.

#### Sales Per Hour
We analyze sales per hour and present the results.

### Product Analysis

#### What Product Sold the Most?
We identify the product that sold the most and share our findings.

#### Top Products for Each City
We determine the top-selling products for each city and provide insights.

#### Top 5 Products with the Highest Revenue for Each City
We present the top 5 products with the highest revenue for each city.

#### What Products Are Most Often Sold Together?
We analyze product associations to identify which products are most frequently sold together.

#### What Percentage of Orders Include Multiple Products?
We calculate the percentage of orders that include multiple products.

### Order Value Analysis

#### What Was the Highest Single-Order Value?
We identify the highest value for a single order.

### City and Revenue Analysis

#### What City with Highest Revenue?
We determine the city with the highest revenue and provide insights.

#### What City Sold the Most Products?
We identify the city that sold the most products.

### State Analysis

#### What Is the Distribution of States?
We analyze the distribution of states in the dataset.

## Conclusion
In conclusion, our data analysis of sales data has provided valuable insights that can guide decision-making across various aspects of the business. These insights include the identification of peak sales months, best-selling products, top revenue-generating cities, and more. The business can make informed decisions to optimize operations, enhance marketing efforts, and maximize revenue. Continued analysis and monitoring of sales data will be crucial for adapting to changing market dynamics and maintaining a competitive edge.
