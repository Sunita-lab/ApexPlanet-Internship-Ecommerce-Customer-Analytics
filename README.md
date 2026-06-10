# ApexPlanet Internship - E-Commerce Customer Analytics

## Task 1: Data Cleaning & Preprocessing

### Objective
Clean and preprocess a real-world e-commerce transaction dataset by identifying missing values, duplicate records, and data quality issues.

### Dataset
Online Retail Dataset

### Tools Used
- Python
- Pandas
- PyCharm

### Dataset Overview
- Original Shape: (541909, 8)
- Cleaned Shape: (535187, 8)

### Data Quality Issues Found

#### Missing Values
- Description: 1454 missing values (0.27%)
- CustomerID: 135080 missing values (24.93%)

#### Duplicate Records
- 5268 duplicate rows identified and removed

#### Additional Observations
- Negative Quantity values observed
- Negative UnitPrice values observed
- These may represent returns, cancellations, or refund transactions

### Cleaning Steps Performed
1. Loaded dataset using Pandas
2. Explored dataset structure
3. Identified missing values
4. Calculated missing value percentages
5. Detected duplicate records
6. Removed duplicate records
7. Removed rows with missing Description values
8. Exported cleaned dataset

### Output
- cleaned_online_retail.csv