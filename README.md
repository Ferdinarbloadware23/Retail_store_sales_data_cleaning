# Retail Store Sales Analysis & Data Cleaning

![Dashboard Preview](your_screenshot_link_here)

## Overview

This project focuses on transforming a raw, "dirty" retail dataset into a reliable analytical report. The main goal was to ensure all sales figures and categories were accurate before performing any analysis.

The objective is to handle missing values, fix data types, and build an interactive dashboard to support better business decisions.

**Period**: 2022 - 2025
**Tools**: Microsoft Excel (Advanced Formulas, Pivot Tables, Slicers, Timelines)

---

## Objectives

- Restore missing "Price Per Unit" data using mathematical logic
- Standardize "Transaction Date" from text format to valid date objects
- Categorize blank product entries as "Unknown" to maintain reporting integrity
- Create an interactive dashboard for real-time sales monitoring

---

## Data Cleaning Process

I followed a professional data analyst workflow (Ask, Prepare, Process, Analyze) to fix the dataset:

1. **Converting Text to Numbers**: Used "Text to Columns" to fix currency and date formats that were stored as text.
2. **Recovering Missing Prices**: Applied the formula `=IF(ISBLANK(E7); G7/F7; E7)` to fill empty price cells based on total spent and quantity.
3. **Handling Blanks**: Identified empty cells in Category and Item columns and labeled them as "Unknown" using `Go To Special > Blanks`.
4. **Data Validation**: Removed duplicate transactions to ensure revenue figures were not inflated.

---

## Key Features & Insights

The final dashboard allows users to explore:
- **Sales by Category**: Identify top-performing product lines.
- **Payment Method Distribution**: Track the most used payment options (Cash, Credit Card, Digital Wallet).
- **Interactive Slicers**: Filter data by Category, Payment Method, and Location instantly.
- **Time Intelligence**: Monitor sales trends across different Years, Quarters, and Months using the Timeline tool.

---

## Dataset

Characteristics:
- **Source**: Retail Store Sales Dataset (Kaggle)
- **Fields**: Transaction ID, Customer ID, Category, Item, Price, Quantity, Total Spent, Method, Location, Date, Discount
