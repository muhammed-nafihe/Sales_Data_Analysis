# Sales Data Analysis

## Overview
This project analyzes e-commerce sales data to derive valuable insights, detect trends, and support data-driven decision-making. The dataset includes transaction details such as order dates, product names, purchase addresses, and sales amounts.

## Objectives
- Clean and preprocess the raw sales data
- Perform exploratory data analysis (EDA) to identify key trends and patterns
- Engineer features to improve data quality
- Visualize the insights using Python libraries

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

