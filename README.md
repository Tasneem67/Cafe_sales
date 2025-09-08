☕ Cafe Sales Data Analysis
📖 Project Overview
This project involves a comprehensive analysis of a cafe's sales data to uncover business insights, identify trends, and understand customer behavior. The analysis is conducted using a Jupyter Notebook (Cafe.ipynb) and leverages Python's powerful data science stack, including pandas, numpy, matplotlib, and seaborn.

The workflow follows a standard data analysis pipeline: loading the data, assessing its quality, cleaning and preprocessing it, performing exploratory data analysis (EDA), and finally, generating visualizations to communicate key findings.

📊 Dataset
The analysis is based on the cleaned_cafe_sales.csv file, which contains 10,000 transactions with the following columns:

Transaction ID: A unique identifier for each transaction.

Item: The product purchased (e.g., Coffee, Cake, Cookie, Salad, Smoothie, etc.).

Quantity: The number of units purchased.

Price Per Unit: The cost of a single unit of the item.

Total Spent: The total amount spent for the item in the transaction (Quantity * Price Per Unit).

Payment Method: The method of payment (Cash, Credit Card, Digital Wallet, Unknown).

Location: Where the transaction took place (In-store, Takeaway, Unknown).

Transaction Date: The date of the transaction.

🛠️ Tech Stack
Language: Python

Libraries:

pandas - Data manipulation and analysis

numpy - Numerical computations

matplotlib - Creating static visualizations

seaborn - Creating statistical visualizations

datetime & calendar - Handling date-time objects

🔍 Analysis Steps
The Jupyter Notebook is structured into the following main sections:

1. Data Assessment
Visual Review: Initial inspection of the dataset using .head(), .sample(), and .tail() to understand its structure and content.

Programmatic Checks: Using .info(), .isnull().sum(), and .describe() to identify data types, missing values, duplicates, and basic statistics.

2. Data Cleaning
Handling Missing Values: Rows with null values in critical columns (Item, Quantity, Price Per Unit, Total Spent) were dropped.

Correcting Data Types: The Transaction Date column was converted to a datetime object for time-based analysis.

Feature Engineering: New columns were created for easier analysis:

Month, Day, Day_Name, Hour extracted from the transaction date.

The Item column was slightly modified for consistency (e.g., replacing '/' with '&').

3. Exploratory Data Analysis (EDA)
Key questions explored include:

What are the top-selling items by quantity?

Which items generate the most revenue?

What are the monthly sales trends?

How is the price of items distributed?

4. Visualization
The notebook includes various visualizations to illustrate the findings, such as:

Box plots to show the distribution of item prices.

Line charts to visualize sales trends over time.

📈 Key Insights (Summary)
Top Selling Items (by Quantity): Coffee, Salad, and Tea are the most frequently sold items.

Top Revenue Generating Items: Despite not being the top seller by quantity, Salad generates the highest total revenue, followed by Sandwich and Smoothie. This suggests Salad has a higher profit margin or price point.

Sales Trends: The data shows clear monthly trends, which can be used for inventory planning and staffing.
