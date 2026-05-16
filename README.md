# 📊 UK E-Commerce Sales Analysis Dashboard (Power BI)

# 📑 Table of Contents

1. Project Overview
2. Project Objectives
3. Tools & Technologies Used
4. Dataset Information
5. Data Cleaning & Preparation
6. Dashboard Pages
7. Business Questions Answered
8. DAX Measures Used
9. Dashboard Design Approach
10. Challenges Encountered
11. Business Recommendations
12. Future Improvements
13. Conclusion
14. Dashboard Preview
15. Author
16. Project Status

## 📌 Project Overview

This project focuses on analyzing an e-commerce transactional dataset to uncover insights related to sales performance, customer purchasing behavior, product trends, and regional sales distribution.

The project was completed as part of a data analytics internship program and was designed to answer key business questions using Power BI and Power Query.

The dashboard was built to support business decision-making through interactive visualizations and KPI monitoring.

---

# 🎯 Project Objectives

The main objectives of this project were to:

* Analyze overall sales performance
* Identify top-performing products
* Understand customer purchasing behavior
* Discover sales trends over time
* Detect unusual transactions and outliers
* Identify top revenue-generating countries
* Build an interactive business dashboard

---

# 🛠️ Tools & Technologies Used

| Tool        | Purpose                               |
| ----------- | ------------------------------------- |
| Power BI    | Dashboard development & visualization |
| Power Query | Data cleaning & transformation        |
| DAX         | KPI calculations and measures         |

---

# 📂 Dataset Information

The dataset contains transactional records from an online retail store, including:

* Invoice details
* Product descriptions
* Quantities purchased
* Unit prices
* Customer IDs
* Transaction dates
* Countries

Dataset source:

* E-commerce transactional dataset from Kaggle

---

# 🧹 Data Cleaning & Preparation (Power Query)

Data preprocessing and transformation were performed using Power Query inside Power BI.

The following cleaning steps were carried out:

## ✅ Removed Duplicate Records

Duplicate rows were removed to improve data quality and avoid inaccurate aggregations.

## ✅ Corrected Data Types

Relevant columns were converted into appropriate data types:

| Column      | Data Type      |
| ----------- | -------------- |
| Quantity    | Whole Number   |
| UnitPrice   | Decimal Number |
| InvoiceDate | Date/Time      |
| CustomerID  | Text           |

## ✅ Created Revenue Column

A calculated revenue field was created using:

Revenue = Quantity × Unit Price

This column was used throughout the dashboard for sales analysis.

## ✅ Date Transformation

Date fields were transformed to support:

* Monthly trend analysis
* Day-of-week analysis
* Hourly sales analysis

---

# 📈 Dashboard Pages

The Power BI dashboard was divided into multiple analytical pages for better storytelling and user experience.

---

# 1️⃣ Executive Overview

This page provides a high-level overview of overall business performance.

## KPI Cards

* Total Revenue
* Total Orders
* Total Customers
* Total Products
* Average Order Value

## Visualizations

* Revenue Trend Over Time (Line Chart)
* Revenue by Country (Bar Chart)
* Country Sales Map
* Top Products by Revenue
* Top Customers by Spending
* Sales by Day of Week

## Key Insights

* Revenue was concentrated among a few top-performing products.
* Certain countries generated significantly higher revenue than others.
* Sales activity fluctuated across different days and months.

---

# 2️⃣ Product Analysis

This page focused on product-level performance analysis.

## Visualizations

* Top Products by Revenue
* Most Sold Products by Quantity
* Low Performing Products Table
* Product Contribution Treemap
* Quantity Distribution Histogram

## Key Insights

* A small number of products generated the majority of sales revenue.
* Some products recorded very low sales and appeared infrequently.
* Bulk purchases contributed significantly to overall quantity sold.

---

# 3️⃣ Customer Insights

This page analyzed customer purchasing behavior.

## Visualizations

* Top Customers by Spending
* Customer Revenue Distribution
* Orders Per Customer Scatter Plot
* Customer Type Analysis

## Key Insights

* High-value customers contributed a significant percentage of total revenue.
* Customer spending patterns varied widely.
* Some customers made frequent purchases while others purchased occasionally.

---

# 4️⃣ Transaction Analysis

This page explored transactional trends and unusual purchase behavior.

## Visualizations

* Monthly Sales Trend
* Sales by Hour
* Sales by Day of Week
* Quantity vs Unit Price Scatter Plot
* Country Sales Analysis

## Key Insights

* Peak shopping periods were identified during specific hours.
* Outlier transactions revealed unusually large purchases.
* Sales trends showed fluctuations across months.

---

# 📊 Key Business Questions Answered

The analysis successfully answered the following business questions:

✅ What is the total revenue generated?

✅ Which products generate the most revenue?

✅ Which products are sold the most by quantity?

✅ Which products generate low sales?

✅ Who are the top customers based on spending?

✅ What are the sales trends over time?

✅ Which countries generate the highest sales?

✅ Are there unusual transactions or outliers?

---

# 📌 DAX Measures Used

## Total Revenue

```DAX
Total Revenue = SUM('Table'[Revenue])
```

## Total Orders

```DAX
Total Orders = DISTINCTCOUNT('Table'[InvoiceNo])
```

## Total Customers

```DAX
Total Customers = DISTINCTCOUNT('Table'[CustomerID])
```

## Average Order Value

```DAX
Average Order Value =
DIVIDE([Total Revenue],[Total Orders])
```

---

# 🎨 Dashboard Design Approach

The dashboard was designed using modern business intelligence best practices:

* Dark sidebar navigation
* Consistent color palette
* Interactive slicers
* Multi-page navigation
* Clear KPI positioning
* Decision-oriented layout
* User-friendly storytelling

---

# 📌 Challenges Encountered

During the project, several challenges were encountered:

* Large dataset handling
* Power BI performance lag
* Data cleaning limitations on low hardware resources
* Managing long product descriptions
* Map visualization inconsistencies

These challenges were addressed through Power Query optimization and dashboard restructuring.

---

# 📈 Business Recommendations

Based on the analysis, the following recommendations were made:

* Focus inventory planning on top-performing products
* Improve marketing strategies for low-selling products
* Develop customer retention programs for high-value customers
* Monitor unusual transactions for operational insights
* Optimize sales efforts in high-performing countries

---

# 🚀 Future Improvements

Although the project was successfully completed using Power BI and Power Query, several future improvements have been planned.

## Planned Improvements

### 🔹 Python Exploratory Data Analysis (EDA)

A more detailed exploratory data analysis using Python and Jupyter Notebook is planned for future updates. Due to temporary laptop performance limitations during the internship submission period, the Python EDA section could not be fully completed.

Future Python analysis will include:

* Advanced statistical analysis
* Correlation analysis
* Additional visualizations
* Customer segmentation analysis
* Time-series analysis
* Automated reporting

### 🔹 Dashboard Redesign & Optimization

The current dashboard structure was developed under limited time constraints. Future improvements will focus on:

* More advanced UI/UX design
* Enhanced interactivity
* Better mobile responsiveness
* Improved visual storytelling
* Advanced DAX calculations
* Additional KPI tracking
* Performance optimization

### 🔹 SQL Integration

Future versions of the project will include:

* SQL business queries
* Database integration
* Data warehouse modeling
* Advanced sales reporting

---

# ✅ Conclusion

This project successfully analyzed e-commerce transactional data using Power BI and Power Query.

The dashboard provides valuable insights into:

* Sales performance
* Product trends
* Customer behavior
* Revenue distribution
* Transaction patterns

The analysis demonstrates how business intelligence tools can support data-driven decision-making and improve business performance.

---

# 📷 Dashboard Preview

(Add your dashboard screenshots here)

---

# 🔗 Author

## Maduabuchi Goodness Chidera

A smart Data Analyst skilled in:

* Excel
* SQL
* Power BI
* Python
* Data Visualization
* Business Intelligence

---

# 📌 Project Status

✅ Completed
