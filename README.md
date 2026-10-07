# SWYNEX Final Data Analytics Project

## FMCG Retail Sales Analytics

This project presents a complete data analytics workflow developed as part of my **Data Analyst Internship at SWYNEX Technologies**.

The project covers the complete journey from raw and messy transaction data to a cleaned dataset, exploratory analysis, business insights, and an interactive Power BI dashboard.

---

## 📌 Project Overview

The objective of this project is to analyze FMCG retail transaction data and identify useful patterns in:

- Revenue performance
- Product categories
- Countries
- Payment methods
- Purchase quantities
- Monthly sales trends

The final outcome is an interactive Power BI dashboard that allows users to explore the analyzed data using filters and visualizations.

---

## 🎯 Problem Statement

Retail transaction datasets can contain missing values, inconsistent categorical values, invalid records, and data stored in unsuitable formats.

The goal of this project is to:

1. Clean and prepare the raw FMCG transaction data.
2. Perform exploratory data analysis to identify important patterns.
3. Extract meaningful business insights.
4. Build an interactive dashboard for clear data-driven reporting.

---

## 📊 Dataset Information

The dataset contains FMCG retail transaction records with information about customers, products, transactions, prices, quantities, dates, countries, and payment methods.

### Original Dataset

- **Rows:** 1,800
- **Columns:** 10

### Original Columns

- transaction_id
- customer_name
- email
- age
- country
- product_category
- unit_price
- quantity
- transaction_date
- payment_method

### Final Cleaned Dataset

- **Rows:** 1,480
- **Columns:** 11
- Added column: `revenue`

The final dataset contains transaction records across 2024–2026.

---

# 🧹 1. Data Cleaning & Preparation

The raw dataset contained several data quality issues that were addressed before analysis.

### Cleaning steps performed

- Standardized country names and categorical values.
- Standardized product category names.
- Standardized payment method values.
- Converted `unit_price` into a numeric format.
- Handled missing unit prices using the mean.
- Removed records containing negative quantities.
- Filled missing quantities using the median.
- Filled missing ages using the mean.
- Removed records with missing transaction dates.
- Converted `transaction_date` into datetime format.
- Created a new `revenue` column.

### Revenue Calculation
Revenue = Unit Price × Quantity
After cleaning, the dataset contained 1,480 valid transaction records.

📈 2. Exploratory Data Analysis

Exploratory Data Analysis was performed to understand transaction patterns and revenue performance.

The analysis included:

Descriptive statistics
Product category analysis
Country-wise revenue analysis
Payment method analysis
Monthly revenue trends
Quantity-wise revenue analysis
Unit price vs revenue analysis
Outlier detection
🔎 Key EDA Findings
Product Categories

Electronics generated the highest total revenue among the product categories.

Product Category	Revenue
Electronics	₹1,733,594.72
Groceries	₹984,612.96
Fashion	₹797,580.21
Home	₹571,879.03
Countries

Nigeria recorded the highest total revenue.

Country	Revenue
Nigeria	₹1,475,058.34
United States	₹1,173,956.64
Ghana	₹577,942.35
United Kingdom	₹487,940.40
Turkey	₹372,769.19

The United Kingdom had the highest average revenue per transaction at approximately ₹2,993.50.

Payment Methods

Card payments generated the highest total revenue and represented the largest number of transactions.

Payment Method	Revenue
Card	₹2,295,070.96
Cash	₹954,148.44
Transfer	₹838,447.52
Quantity Analysis

Average revenue increased as the quantity purchased increased.

Quantity	Average Revenue
1	₹1,158.23
2	₹2,262.48
3	₹3,329.52
4	₹4,670.63
5	₹5,291.10
Monthly Revenue

The highest monthly revenue in the analyzed dataset was recorded in August 2025, with approximately ₹2,54,070.12.

The lowest was recorded in February 2026, with approximately ₹78,702.09.

Note: February 2026 may represent a partial period in the dataset.

Outlier Analysis

Using the IQR method:

Q1 = ₹1,133.52
Q3 = ₹3,600.00
Upper outlier threshold = ₹7,299.72
Number of high-revenue outliers = 105
Maximum revenue = ₹12,500

These records were retained because the higher values were consistent with higher unit prices and quantities rather than clearly invalid data.

📊 3. Interactive Power BI Dashboard

The cleaned and analyzed data was used to create an interactive Power BI dashboard.

Dashboard KPIs
Total Revenue: ₹4,087,666.92
Total Transactions: 1,480
Average Revenue: ₹2,761.94
Total Quantity: 3,656
Dashboard Visualizations
Revenue by Product Category
Revenue by Country
Monthly Revenue Trend
Revenue by Payment Method
Average Revenue by Quantity
Interactive Filters

The dashboard includes filters for:

Country
Product Category
Payment Method
Year

Selecting a filter dynamically updates the dashboard visuals.

💡 4. Key Business Insights

Based on the analysis:

Electronics is the strongest product category in terms of total revenue.
Nigeria contributes the highest total revenue among the analyzed countries.
Card payments are the dominant payment method by transaction activity and revenue.
Higher purchase quantities are associated with higher average transaction revenue.
Higher unit-price groups contribute substantially more revenue per transaction.
Revenue varies considerably across months, indicating changes in sales activity over time.
High-revenue transactions are generally associated with higher quantities and unit prices.
🛠️ Tools & Technologies
Python
Pandas
Jupyter Notebook / Google Colab
Power BI
Power Query
DAX
CSV
📂 Repository Contents
SWYNEX-Final-Data-Analytics-Project
│
├── README.md
├── dirty_transactions_dataset.csv
├── cleaned_fmcg_dataset.csv
├── SWYNEX_Task_1_Data_Cleaning.ipynb
├── SWYNEX_Task_2_Exploratory_Data_Analysis.ipynb
├── Dashboard.pbix
└── dashboard.png
🎓 Learning Outcomes

Through this project, I gained practical experience in:

Data cleaning and preprocessing
Handling missing and invalid data
Exploratory data analysis
Statistical and categorical analysis
Identifying business insights
Data visualization
Power BI dashboard development
Creating interactive filters
Presenting analytical findings in a business-friendly format
✅ Conclusion

This project demonstrates a complete data analytics workflow, starting from raw FMCG transaction data and progressing through data cleaning, exploratory analysis, insight generation, and interactive dashboard development.

The final dashboard provides a clear view of revenue performance across products, countries, payment methods, quantities, and time periods.

The project helped strengthen practical skills in Python-based data analysis and Power BI visualization while demonstrating how raw transactional data can be transformed into meaningful business insights.

🏢 Internship

Data Analyst Internship | SWYNEX Technologies

This project was completed as part of the SWYNEX Technologies Data Analyst Internship.

#SWYNEX #DataAnalytics #PowerBI #Python #DataVisualization #Internship
