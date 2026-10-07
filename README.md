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

```text
Revenue = Unit Price × Quantity
