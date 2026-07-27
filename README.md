# E-Commerce Customer Analytics

**Data Analytics Internship — ApexPlanet Software Pvt. Ltd.**

Author: **Sunita Satpathy**

---

## Overview

This repository documents a four-part data analytics internship project built around an e-commerce transactions dataset. The project follows the complete analytics lifecycle — from raw data to a statistically validated business narrative:

1. **Data Wrangling** — cleaning and preparing a raw dataset for analysis
2. **Exploratory Data Analysis & Business Intelligence** — uncovering patterns and answering business questions with SQL
3. **KPI Definition & Interactive Dashboarding** — building an executive-ready Power BI dashboard
4. **Data Storytelling & Statistical Validation** — synthesizing findings into a business story and validating a key insight with hypothesis testing

Each task builds on the previous one's output, culminating in a final presentation deck for stakeholders.

---

## Tech Stack

| Category | Tools |
|---|---|
| Language | Python |
| Data Manipulation | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Database / Querying | SQLite (via `sqlite3`), SQL |
| Statistics | SciPy (`scipy.stats`) |
| Dashboarding | Microsoft Power BI |
| Environment | Jupyter Notebook |
| Version Control | GitHub |

---

## Project Structure

```
├── data/
│   ├── customer.xlsx                          # Raw dataset used in Task 1
│   └── ApexPlanet_DataAnalytics_Dataset.xlsx   # Raw dataset used in Task 2–4
│
├── task 01 - data wrangling/
│   └── task1_data_wrangling.ipynb
│
├── task 02 - EDA and business analytics/
│   ├── eda_and_business_analytics.ipynb
│   └── cleaned_ecommerce_data.csv              # Analysis-ready dataset used by Tasks 3 & 4
│
├── task 03 - business intelligence dashboard/
│   └── task_03_business_intelligence_dashboard.ipynb
│
├── task 04 - data storytelling and statistical validation/
│   └── task_04_data_storytelling_and_statistical_validation.ipynb
│
└── README.md
```

---

## Task 1 — Data Immersion & Wrangling

**Objective:** Acquire, clean, and prepare a raw transactional dataset for analysis.

**What was done:**
- Loaded a raw online retail transactions dataset (541,909 rows × 8 columns)
- Profiled missing values (`Description`: 1,454 missing; `CustomerID`: 135,080 missing) and duplicate records (5,268 duplicates)
- Removed duplicates and rows with missing `Description`
- Converted `InvoiceDate` to proper datetime format
- Built a data dictionary documenting each column's type, meaning, and business relevance
- Exported a cleaned, analysis-ready dataset (535,187 rows × 8 columns)

**Deliverables:** Data dictionary, cleaning script, cleaned dataset, LinkedIn walkthrough video

---

## Task 2 — Exploratory Data Analysis & Business Intelligence

**Objective:** Uncover patterns and trends in customer purchasing behaviour, and build SQL proficiency for business-question answering.

**What was done:**
- Profiled a 1,000-row e-commerce dataset (12 columns): missing `Age` (20) and `City` (13) handled via median imputation and an "Unknown" category respectively
- Validated `Total_Sales = Quantity × Unit_Price` across all records
- Engineered `Month` and `Age_Group` features for time-based and demographic analysis
- Loaded the cleaned data into SQLite and answered 7 business questions via SQL — top products/categories by revenue, top customers, city-wise sales, monthly trend, gender-wise revenue, and average order value
- Performed univariate analysis (age, quantity, sales distributions) and correlation analysis between numeric fields
- Built a static mock-up proposing key metrics for a dashboard

**Key Findings:**
- **Electronics** is the top revenue category (₹5.08 Cr), more than double any other category
- **Laptop** leads product revenue (₹2.54 Cr); **Mobile** leads unit volume (1,008 units)
- Sales peak in **March** and dip in **August–September**
- **Total_Sales** correlates moderately with both `Quantity` (r = 0.65) and `Unit_Price` (r = 0.69); `Age` shows negligible correlation

**Deliverables:** EDA report, SQL queries with results, LinkedIn showcase video

---

## Task 3 — Deep-Dive Analysis & Interactive Dashboarding

**Objective:** Define core KPIs and build a functional, interactive Power BI dashboard.

**KPIs Defined:**

| KPI | Value |
|---|---|
| Total Sales | ₹13,93,99,439.65 |
| Total Orders | 992 |
| Average Order Value (AOV) | ₹1,40,523.63 |
| Average Sales per Customer | ₹1,47,201.10 |
| Repeat Purchase Rate | 5.49% |

**Deep-Dive: Customer Segmentation**
- **36–45** age group is the highest-revenue segment (₹3.15 Cr), followed by 26–35
- Male customers generated marginally higher total sales (₹7.25 Cr) than female customers (₹6.69 Cr)
- **Patna** leads city-wise revenue, closely followed by Kolkata, Bengaluru, and Mumbai

**Dashboard:** Built in Microsoft Power BI with 4 pages — Executive Overview, Customer Segmentation, Product Analysis, and Geographic Analysis — with an interactive month slicer.

**Deliverables:** Deep-dive report, live dashboard link, LinkedIn demo video

---

## Task 4 — Data Storytelling & Statistical Validation

**Objective:** Synthesize all prior analysis into a business narrative and statistically validate a key observation.

**Hypothesis Test — Is the Gender Sales Gap Statistically Significant?**

| Parameter | Value |
|---|---|
| Test | Independent Two-Sample T-Test (Welch's, unequal variance) |
| H₀ | No significant difference in average sales between male and female customers |
| H₁ | A significant difference exists |
| Significance Level (α) | 0.05 |
| Male customers (n) | 511 |
| Female customers (n) | 489 |
| T-statistic | 0.6826 |
| P-value | 0.4950 |
| **Decision** | **Fail to reject H₀** |

**Conclusion:** The observed gender sales gap is not statistically significant — gender alone is not a reliable factor for customer targeting. Marketing decisions should instead be grounded in validated signals such as product category, age group, city, and seasonal trends.

**Deliverables:** Final presentation deck, hypothesis testing summary, LinkedIn stakeholder presentation video

---

## Business Recommendations

1. **Double down on Electronics** — prioritize inventory and promotions; it drives 2x the revenue of any other category
2. **Target the 26–45 age segment** — the core revenue-driving demographic, not gender
3. **Address the August–September slump** — plan promotions ahead of the seasonal dip; sustain the Oct–Dec rebound
4. **Invest in retention** — a 5.49% repeat-purchase rate signals most customers are one-time buyers
5. **Balance Laptop & Mobile inventory strategy** — Laptop drives revenue, Mobile drives volume
6. **Validate before deciding** — continue statistical testing on new patterns before they shape marketing spend

---

## How to Run

1. Clone the repository and ensure Python 3.x with `pandas`, `numpy`, `matplotlib`, `seaborn`, and `scipy` installed
2. Run notebooks in order: Task 1 → Task 2 → Task 3 → Task 4 (each depends on the cleaned dataset produced by the previous task)
3. Open the Power BI dashboard file to explore the interactive KPIs
4. Refer to the Task 4 presentation deck for the complete stakeholder-facing summary

---

## Acknowledgements

This project was completed as part of the **Data Analytics Internship at ApexPlanet Software Pvt. Ltd.**