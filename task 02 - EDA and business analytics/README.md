# E-Commerce Customer Analytics
### ApexPlanet Software Pvt. Ltd. – Data Analytics Internship (Task 2)

## Project Overview

This project focuses on analyzing an E-Commerce Customer Dataset using Data Analytics techniques.

The objective was to perform:

- Data Cleaning
- Data Validation
- Feature Engineering
- Exploratory Data Analysis (EDA)
- Data Visualization
- Business Insight Generation

The project demonstrates how raw business data can be transformed into meaningful insights that support data-driven decision-making.

---

## Dataset Information

The dataset contains customer purchase records including:

- Customer Information
- Product Details
- Order Information
- Sales Data
- Demographic Attributes
- Location Information

### Dataset Size

- Rows: 1000
- Columns: 12

### Key Features

| Feature | Description |
|----------|------------|
| Order_ID | Unique order identifier |
| Order_Date | Date of purchase |
| Customer_ID | Unique customer identifier |
| Customer_Name | Customer name |
| Age | Customer age |
| Gender | Customer gender |
| City | Customer location |
| Product | Purchased product |
| Category | Product category |
| Quantity | Quantity purchased |
| Unit_Price | Price per unit |
| Total_Sales | Total order value |

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Data Cleaning & Preparation

The following preprocessing steps were performed:

### Missing Value Handling

- Missing values in Age were filled using Median Imputation.
- Missing values in City were replaced with "Unknown".

### Data Validation

- Duplicate records were checked and verified.
- Data types were inspected and corrected.

### Feature Engineering

Two additional features were created:

- Month
- Age_Group

These features were used for time-based and demographic analysis.

---

## Exploratory Data Analysis (EDA)

### Customer Demographics

- Age Distribution
- Age Group Distribution
- Sales by Gender
- Sales by Age Group

### Sales Analysis

- Total Sales Distribution
- Sales Box Plot
- Monthly Sales Trend

### Product & Category Analysis

- Category Distribution
- Total Sales by Category
- Average Sales by Category
- Top Products by Revenue
- Products by Quantity Sold

### Customer Analysis

- Top Customers by Revenue

### Geographic Analysis

- Total Sales by City

### Advanced Analytics

- Monthly Sales Heatmap
- Correlation Analysis

---

## Key Findings

- Electronics emerged as the highest revenue-generating category.
- Grocery recorded the highest average sales per transaction.
- March and November showed strong sales performance, while September had the lowest sales.
- Customer_335 generated the highest revenue among customers.
- Male customers contributed slightly higher sales than female customers.
- The 36–45 age group generated the highest revenue.
- Patna was the highest-performing city in terms of total sales.
- Laptop generated the highest revenue, while Mobile recorded the highest sales volume.
- Quantity and Unit Price showed moderate positive correlation with Total Sales.
- Customer age showed minimal correlation with purchasing behavior.

---

## Business Recommendations

- Prioritize Electronics inventory and promotions.
- Implement targeted campaigns during low-performing months.
- Focus customer retention efforts on high-value customers.
- Strengthen marketing for the 26–45 age segment.
- Expand engagement strategies in high-performing cities.
- Balance inventory between high-volume and high-revenue products.

---

## Project Outcome

This project successfully transformed raw e-commerce transaction data into actionable business insights through:

- Data Cleaning
- Feature Engineering
- Exploratory Data Analysis
- Data Visualization
- Business Intelligence Reporting

The findings can support inventory planning, customer segmentation, marketing strategy, and revenue optimization.

---

## Repository Structure

```text
├── eda_and_business_analytics.ipynb
├── cleaned_ecommerce_data.csv
├── README.md
└── dataset.csv
```

---

## Author

Sunita Satpathy

Data Analytics Internship Project

ApexPlanet Software Pvt. Ltd.