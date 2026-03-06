
NumPy Data Analysis Practice Dataset

Overview

This project provides a demo dataset (2000 rows × 10 columns) designed for practicing NumPy-based data analysis.
It simulates a small sales and customer transaction dataset that analysts might work with in real business scenarios.
The goal of this dataset is to help learners practice:
•	NumPy array operations
•	Vectorized calculations
•	Filtering and indexing
•	Statistical analysis
•	Business metric calculations
This dataset is suitable for beginner to intermediate Data Analyst practice.

Dataset Information
File: demo_sales_data_2000_rows.csv
Rows: 2000
Columns: 10
Each row represents a customer purchase transaction.

Column Description
Column Name	Description
customer_id	Unique ID for each customer
age	Customer age
gender	Gender (0 = Female, 1 = Male)
region	Region code (1–5)
units_sold	Number of units purchased
price_per_unit	Price of each unit
discount_percent	Discount applied to the order
rating	Customer rating (1–5 scale)
is_returned	Whether product was returned (1 = Yes, 0 = No)
days_to_delivery	Number of days required for delivery

Loading the Dataset Using NumPy
import numpy as np

data = np.genfromtxt(
    "demo_sales_data_2000_rows.csv",
    delimiter=",",
    skip_header=1
)

print(data.shape)
Expected Output
(2000, 10)

Learning Objectives
By working with this dataset you will practice:
•	Array slicing
•	Boolean filtering
•	Vectorized calculations
•	Statistical operations
•	Business KPI analysis
•	Data transformation

Practice Questions (NumPy)
Below are 25 practical data analysis questions you can solve using NumPy.
Basic Exploration
1.	Find the shape of the dataset
2.	Count total rows
3.	Count total columns
4.	Find average customer age
5.	Find minimum and maximum age
Sales Analysis
6.	Calculate total units sold
7.	Calculate average price per unit
8.	Calculate total revenue before discount
9.	Calculate discount amount per transaction
10.	Calculate net revenue
Revenue Analysis
11.	Calculate total net revenue
12.	Calculate average net revenue
13.	Identify transactions where units sold > 30
14.	Calculate average customer rating
15.	Count total returned orders
Customer Insights
16.	Calculate return rate (%)
17.	Calculate average delivery time
18.	Find orders delivered within 3 days
19.	Calculate revenue from transactions with ≥15% discount
20.	Compare average revenue by gender
Advanced Analysis
21.	Find region with highest average revenue
22.	Calculate standard deviation of price
23.	Find top 5 transactions by net revenue
24.	Calculate percentage of customers rating ≥ 4
25.	Add net revenue as a new column to the dataset

Example Calculation
Example: Calculate Revenue
units = data[:,4]
price = data[:,5]

revenue = units * price
Example: Net Revenue
discount = revenue * (data[:,6] / 100)
net_revenue = revenue - discount

Skills Practiced
Working with this dataset will strengthen:
•	NumPy fundamentals
•	Data filtering
•	Business KPI analysis
•	Analytical thinking
•	Python for Data Analysis

Recommended Learning Path
To become a Data Analyst, combine this practice with:
•	SQL
•	Pandas
•	Excel
•	Data Visualization (Power BI / Tableau)

Author
Practice dataset for NumPy Data Analysis learning.

License
Free to use for learning and educational purposes.

