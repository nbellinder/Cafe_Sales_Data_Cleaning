# Cafe Sales Data Cleaning
## Overview
The Dirty Cafe Sales dataset contains 10,000 rows of synthetic data representing sales transactions in a cafe. This dataset is intentionally "dirty," with missing values, inconsistent data, and errors introduced to provide a realistic scenario for data cleaning.
I will clean the same data in both Excel and SQL to showcase methods in both programs to prepare this data for proper analysis.

## Data Structure & Initial Checks
The Cafe's sales database structure as seen below consists of one table: dirty_cafe_sales with a total row count of 10,000.

![image](https://github.com/user-attachments/assets/c45ee0fd-c37f-41c2-a3f8-5a0785a195e0)

## Data Cleaning
• The original CSV file for the database can be found [here](https://github.com/nbellinder/Cafe_Sales_Data_Cleaning/blob/main/dirty_cafe_sales.csv).

• Targeted SQL queries with explanations used to inspect and clean the data can be found [here](https://github.com/nbellinder/Cafe_Sales_Data_Cleaning/blob/main/SQL%20Dataset%20Cleaning%20Queries).

• An Excel Workbook with the dirty data, cleaned data, and an update log can be found [here](https://github.com/nbellinder/Cafe_Sales_Data_Cleaning/blob/main/dirty_cafe_sales_clean.xlsx).

## Missing Data Handling

• Contextually, many NULL values in **Item**, **Quantity**, **Price Perr Unit**, and **Total Spent** were able to be recovered.

• There needs to be a deeper discussion with Stakeholders about the viability of records that lack 2 or more of: **Quantity**, **Price Per Unit**, and **Total Spent** and if they should be removed from the dataset because of their lack of value.

• There was no reliable way to estimate **Transaction Date** and a lack of supplementry information to find missing **Payment Methods** or **Location**. Because of this, missing values in these fields were made NULL.
