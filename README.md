📊 FMCG Retail Sales Analytics
📌 Project Overview

This project focuses on analyzing FMCG retail transaction data to identify revenue patterns, customer purchasing behavior, product performance, and business trends.

The project follows a complete data analytics workflow, starting from raw transaction data, followed by data cleaning and preprocessing, exploratory data analysis (EDA), and finally the development of an interactive Power BI dashboard.

The objective is to transform raw transactional data into meaningful insights that can support data-driven business decisions.

🎯 Objectives

The main objectives of this project are:

Clean and preprocess raw FMCG transaction data.

Handle missing, invalid, and inconsistent data.

Perform exploratory data analysis.

Analyze revenue across different dimensions.

Identify important sales and business trends.

Create meaningful data visualizations.

Develop an interactive Power BI dashboard.

Present actionable business insights.

🗂️ Dataset

The dataset contains FMCG retail transaction information, including customer, product, pricing, quantity, date, country, and payment details.

Original Dataset

Rows: 1,800

Columns: 10

Columns
Column	Description
transaction_id	Unique transaction identifier
customer_name	Customer name
email	Customer email
age	Customer age
country	Customer country
product_category	Product category
unit_price	Price per unit
quantity	Quantity purchased
transaction_date	Date of transaction
payment_method	Method used for payment
🧹 Data Cleaning & Preprocessing

The raw dataset contained several data-quality issues. The following preprocessing steps were performed:

Standardized categorical values.

Standardized country names.

Standardized product categories.

Standardized payment methods.

Converted unit_price into a numeric data type.

Handled missing unit prices using the mean.

Identified and removed records containing negative quantities.

Handled missing quantities using the median.

Handled missing ages using the mean.

Removed records with missing transaction dates.

Converted transaction_date into the appropriate datetime format.

Created a new revenue column.

Revenue Calculation
Revenue = Unit Price × Quantity


After cleaning, the dataset contained:

1,480 valid transactions

11 columns

📈 Exploratory Data Analysis

Exploratory analysis was performed using Python and Pandas to understand the structure and behavior of the dataset.

The analysis focused on:

Revenue distribution

Product category performance

Country-wise revenue

Payment method performance

Quantity and revenue relationship

Monthly revenue trends

Unit price and revenue relationship

Outlier detection

🔍 Key Findings
🛍️ Revenue by Product Category

Electronics generated the highest total revenue among the analyzed product categories.

Product Category	Revenue
Electronics	₹1,733,594.72
Groceries	₹984,612.96
Fashion	₹797,580.21
Home	₹571,879.03
🌍 Revenue by Country

Nigeria recorded the highest total revenue among the countries in the dataset.

Country	Revenue
Nigeria	₹1,475,058.34
United States	₹1,173,956.64
Ghana	₹577,942.35
United Kingdom	₹487,940.40
Turkey	₹372,769.19

The United Kingdom recorded the highest average revenue per transaction at approximately ₹2,993.50.

💳 Revenue by Payment Method

Card payments generated the highest total revenue.

Payment Method	Revenue
Card	₹2,295,070.96
Cash	₹954,148.44
Transfer	₹838,447.52
📦 Quantity Analysis

The analysis showed a positive relationship between purchase quantity and average transaction revenue.

Quantity	Average Revenue
1	₹1,158.23
2	₹2,262.48
3	₹3,329.52
4	₹4,670.63
5	₹5,291.10
📅 Monthly Revenue

Revenue was also analyzed over time to identify monthly sales patterns and fluctuations.

The highest monthly revenue was recorded in August 2025, while the lowest was recorded in February 2026.

Note: Monthly comparisons should consider the number of records available for each period, particularly where a month may represent a partial reporting period.

📊 Outlier Analysis

The Interquartile Range (IQR) method was used to identify unusually high revenue transactions.

Q1: ₹1,133.52

Q3: ₹3,600.00

Upper Outlier Threshold: ₹7,299.72

High-Revenue Outliers: 105

Maximum Revenue: ₹12,500

The identified high-value transactions were retained because they were not necessarily data errors and could be explained by higher quantities and/or higher unit prices.

📊 Power BI Dashboard

The cleaned dataset was imported into Power BI to create an interactive sales analytics dashboard.

Dashboard KPIs

Total Revenue: ₹4,087,666.92

Total Transactions: 1,480

Average Revenue: ₹2,761.94

Total Quantity: 3,656

Dashboard Visualizations

The dashboard includes:

Revenue by Product Category

Revenue by Country

Monthly Revenue Trend

Revenue by Payment Method

Average Revenue by Quantity

KPI cards for key business metrics

Interactive Filters

Users can filter the dashboard by:

Country

Product Category

Payment Method

Year

These filters allow users to explore the dataset from different business perspectives.

💡 Business Insights

The analysis produced several important insights:

Electronics is the strongest revenue-generating product category.

Nigeria contributes the highest total revenue among the analyzed countries.

Card payments dominate transaction revenue compared with cash and transfer payments.

Higher purchase quantities are associated with higher average revenue.

High-value transactions are generally associated with higher quantities and/or unit prices.

Revenue varies across months, indicating fluctuations in sales activity over time.

Country-level performance varies considerably, providing opportunities for market-specific strategies.

🛠️ Tools & Technologies
Tool	Purpose
Python	Data cleaning and analysis
Pandas	Data manipulation and preprocessing
Jupyter Notebook / Google Colab	Analysis environment
Power BI	Interactive dashboard
Power Query	Data transformation
DAX	Power BI calculations
CSV	Dataset format
📁 Project Structure
FMCG-Retail-Sales-Analytics/
│
├── README.md
│
├── data/
│   ├── dirty_transactions_dataset.csv
│   └── cleaned_fmcg_dataset.csv
│
├── notebooks/
│   ├── SWYNEX_Task_1_Data_Cleaning.ipynb
│   └── SWYNEX_Task_2_Exploratory_Data_Analysis.ipynb
│
├── powerbi/
│   └── Dashboard.pbix
│
└── images/
    └── dashboard.png

📸 Dashboard Preview

Add your Power BI dashboard screenshot here:

![FMCG Sales Dashboard](images/dashboard.png)

📚 Learning Outcomes

Through this project, I developed practical experience in:

Data cleaning and preprocessing

Missing-value treatment

Data validation

Exploratory data analysis

Statistical analysis

Outlier detection

Data visualization

Power BI dashboard development

DAX calculations

Business insight generation

Data storytelling

🚀 Future Improvements

Possible improvements for future versions include:

Customer segmentation analysis.

Profit and margin analysis.

Customer lifetime value analysis.

Product-level performance analysis.

Sales forecasting.

Advanced Power BI DAX measures.

Automated data refresh.

More detailed geographic analysis.

Predictive analytics using machine learning.

🏁 Conclusion

This project demonstrates an end-to-end Data Analytics workflow, from raw FMCG transaction data to a cleaned dataset, exploratory analysis, business insights, and an interactive Power BI dashboard.

The analysis highlights important patterns in product performance, geographic revenue, payment methods, purchase quantities, and sales trends.

Overall, the project demonstrates how data cleaning, analysis, visualization, and business intelligence can be combined to transform raw transactional data into meaningful and actionable insights.

👨‍💻 Author

Data Analyst Portfolio Project

Skills: Python • Pandas • SQL • Power BI • Excel • Data Visualization • Exploratory Data Analysis

⭐ If you found this project useful

Feel free to ⭐ star the repository and explore the notebooks and Power BI dashboard.
