# Retail Store Sales Analysis & Data Cleaning

![Dashboard Preview](dashboard_preview_retailstoresales.png)

## Overview
This project focuses on transforming a raw, "dirty" retail dataset into a reliable analytical report. The primary goal was to ensure data accuracy before performing any analysis, covering everything from handling missing values to standardizing data formats.

The final dashboard is designed to support business decision-making through real-time monitoring of key sales performance metrics.

- **Period**: 2022 - 2025
- **Tools**: Microsoft Excel (Advanced Formulas, Pivot Tables, Slicers, Timeline)

---

## Objectives
- Restore missing "Price Per Unit" data using mathematical logic.
- Standardize "Transaction Date" from text format into valid date objects.
- Categorize blank product entries as "Unknown" to maintain reporting integrity.
- Build an interactive dashboard to monitor key KPI performance.

---

## Data Cleaning Process
I followed a professional Data Analyst workflow (Ask, Prepare, Process, Analyze) to fix the dataset:

1. **Converting Text to Numbers**: Used *Text to Columns* and formatting tools to fix currency and date values stored as text.
2. **Recovering Missing Prices**: Applied the formula `=IF(ISBLANK(E7); G7/F7; E7)` to calculate empty price cells based on Total Spent and Quantity.
3. **Handling Blanks**: Identified empty cells in Category and Item columns and labeled them as "unknown" using *Go To Special > Blanks*.
4. **Data Validation**: Removed or verified duplicate transactions to ensure revenue figures were not inflated.

---

## Key Features & Insights
The final dashboard allows users to explore:

- **Sales by Category**: Identify top-performing product lines. The **Butchers** category is the leading revenue contributor at **$208,118**.
- **Payment Method Distribution**: Track the most frequently used payment options (Cash, Credit Card, Digital Wallet).
- **Interactive Slicers**: Filter data by Location and Payment Method instantly for granular analysis.
- **Time Intelligence**: Monitor monthly and yearly sales trends. A performance peak is observed in **2024** before a decline in early 2025.

---

## Key Metrics Summary
Based on the final analysis, here is the retail performance snapshot:
- **Total Revenue**: $1,552,071
- **Total Transactions**: 12,575
- **Average Order Value (AOV)**: $123

---

## Dataset Characteristics
- **Source**: Retail Store Sales Dataset (Kaggle)
- **Fields**: Transaction ID, Customer ID, Category, Item, Price, Quantity, Total Spent, Payment Method, Location, Transaction Date, Discount Applied.
