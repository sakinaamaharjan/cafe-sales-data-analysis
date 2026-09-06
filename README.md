# Café Sales Data Analysis

## Project Overview

This project focuses on cleaning, exploring, and visualizing a messy café sales dataset using Python and Pandas. The dataset contains 10,000 transaction records with missing values, inconsistent entries, and data quality issues.

The project demonstrates a practical data analysis workflow, from understanding and cleaning raw data to extracting insights and creating visualizations.

## Objectives

1. Identify and understand data quality issues within the dataset.
2. Clean and preprocess the raw café sales data.
3. Handle missing and inconsistent values appropriately.
4. Explore sales patterns and customer purchasing behavior.
5. Analyze product performance and payment methods.
6. Examine changes in sales over time.
7. Identify relationships between numerical variables.
8. Create clear and informative data visualizations.
9. Develop a practical Data Science project for a portfolio.

## Tools and Technologies

1. Python
2. Pandas
3. Matplotlib
4. Seaborn
5. Jupyter Notebook
6. VS Code
7. Git
8. GitHub

## Dataset

The dataset used for this project is the Café Sales dataset, a synthetic dataset designed to simulate real world café transactions.

The dataset contains 10,000 transaction records and includes the following variables:

1. Transaction ID
2. Item
3. Quantity
4. Price Per Unit
5. Total Spent
6. Payment Method
7. Location
8. Transaction Date
9. Month

## Project Workflow

### 1. Data Import

The raw café sales dataset was imported into Python using Pandas.

### 2. Initial Data Understanding

1. Dataset Dimensions
   Checked the number of rows and columns in the dataset.

2. Column Names
   Reviewed all available columns to understand the variables included in the dataset.

3. Data Types
   Checked the data type of each column and identified columns that required conversion.

4. Missing Values
   Identified the number of missing values in each column.

5. Duplicate Values
   Checked the dataset for duplicate records.

6. Unique Values
   Reviewed unique values in categorical columns such as Item, Payment Method, and Location.

7. Descriptive Statistics
   Examined numerical variables using summary statistics such as mean, median, minimum, and maximum values.

### 3. Data Cleaning and Preprocessing

1. Text Cleaning
   Removed unnecessary spaces and standardized text values.

2. Date Conversion
   Converted Transaction Date into the appropriate datetime format.

3. Missing Value Handling
   Examined missing values and handled them according to the type and importance of each variable.

4. Numerical Data Validation
   Compared Quantity, Price Per Unit, and Total Spent to identify inconsistencies.

5. Derived Variables
   Created Month from Transaction Date for time based analysis.

6. Data Validation
   Checked the cleaned dataset for remaining inconsistencies and duplicate records.

### 4. Missing Value Analysis

The main missing values identified in the dataset were:

1. Quantity: 38 missing values
2. Price Per Unit: 38 missing values
3. Total Spent: 40 missing values
4. Transaction Date: 6,458 missing values
5. Month: 6,458 missing values

Missing values were not automatically replaced with arbitrary values.

1. Numerical values were reconstructed only when enough reliable information was available.
2. Missing categorical values were handled without assuming that the most common category was always correct.
3. Transaction dates were not artificially created when they could not be reliably determined.
4. Missing values that could not be reliably reconstructed were retained rather than replaced with invented information.

### 5. Descriptive Analysis

The distribution of Total Spent was examined to understand typical transaction values.

1. Average transaction value: 8.93
2. Median transaction value: 8
3. Minimum transaction value: 1
4. Maximum transaction value: 25

### 6. Exploratory Data Analysis

1. Most Frequently Purchased Products
   Coffee was the most frequently purchased item, while cookies were purchased the least frequently.

2. Product Performance
   Salad generated the highest total spending, while cookies generated the lowest.

3. Sales and Product Comparison
   Although coffee was the most frequently purchased product, it did not generate the highest total spending. This shows that sales frequency and financial performance are not always the same.

4. Payment Methods
   Credit card was the most commonly used payment method.

5. Monthly Analysis
   June recorded the highest total spending, while November recorded the largest decline.

6. Quantity and Total Spending
   The scatter plot showed that higher quantities generally corresponded with higher total spending.

7. Outlier Analysis
   Boxplots were used to identify unusually high or low values in numerical variables.

## Data Visualization

The project includes visualizations for the following areas:

1. Sales by Item
2. Total Spending by Item
3. Monthly Spending Trends
4. Payment Method Analysis
5. Quantity vs Total Spending
6. Numerical Variable Outliers

These visualizations were created using Matplotlib and Seaborn to make patterns, comparisons, and relationships easier to understand.

## Key Findings

1. Coffee was the most frequently purchased product.
2. Salad generated the highest total spending.
3. Cookies had the lowest total spending.
4. Credit card was the most commonly used payment method.
5. June had the highest total spending among transactions with available dates.
6. November showed the largest decline in monthly spending.
7. Higher quantities generally resulted in higher total spending.
8. The most frequently purchased product was not necessarily the product with the highest total spending.

## Recommendations

Based on the analysis, the following recommendations can be considered:

1. Continue monitoring the performance of high performing products such as salad.
2. Investigate why some frequently purchased products do not generate the highest total spending.
3. Monitor payment method preferences to understand customer purchasing behavior.
4. Improve the collection of transaction dates to enable more reliable time based analysis.
5. Maintain consistent data entry practices to reduce missing and inconsistent values.

## Limitations

1. The dataset contains a large number of missing transaction dates, which limits the reliability of long term time based analysis.

2. Monthly spending analysis was conducted using transactions with available transaction dates.

3. The dataset is synthetic and may not accurately represent real café customer behavior.

4. Some missing values could not be reliably reconstructed without making assumptions.

5. The dataset contains Total Spent rather than actual business profit because cost information is not provided. Therefore, the financial analysis in this project refers to total spending rather than net profit.

## Repository Contents

1. dirty_cafe_sales.ipynb
   Contains the complete data cleaning, exploratory analysis, and visualization workflow.

2. dirty_cafe_sales.csv
   Contains the original raw dataset.

3. cleaned_dataset.csv
   Contains the cleaned version of the dataset.

4. README.md
   Contains the documentation for the project, methodology, findings, and limitations.

## What I Learned

1. How to inspect and understand a messy dataset before beginning analysis.
2. How to identify different types of data quality issues.
3. How to handle missing values without unnecessarily changing the original information.
4. How to use Pandas for data cleaning and transformation.
5. How to perform exploratory data analysis to identify useful patterns.
6. How to create visualizations that communicate data driven findings.
7. How to interpret relationships between different variables.
8. How to use Git and GitHub to organize and publish a Data Science project.

## Future Improvements

1. Perform deeper statistical analysis.
2. Build an interactive dashboard using a suitable Business Intelligence tool.
3. Investigate customer purchasing patterns in greater detail.
4. Perform more advanced time series analysis if more complete date information becomes available.
5. Explore predictive modeling using a larger and more reliable dataset.
6. Incorporate additional business variables such as cost and profit if real business data becomes available.

## Author

Sakina Maharjan

Computer Science Student specializing in Data Science
