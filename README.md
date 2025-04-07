# Marketing Campaign Dataset Cleaner

This project provides a Python script to clean a messy marketing campaign dataset. It handles common issues like missing values, inconsistent formatting, and duplicates.

## 📁 Files

- `marketing_campaign_dirty.xlsx` – Raw dataset (input file)
- `clean_data.py` – Python script to clean the dataset
- `marketing_campaign_cleaned.xlsx` – Cleaned dataset (output file)

## 🧹 What the Script Does

- Standardizes column names (lowercase, underscores, removes special chars)
- Removes duplicate rows
- Drops columns with more than 50% missing values
- Fills missing values:
  - Text columns → `'Unknown'`
  - Numeric columns → column median
- Trims whitespace in string values
- (Optional) Converts date columns to proper datetime format

## 🚀 How to Use

### 1. Install dependencies

Make sure you have Python 3 and `pandas` installed:

```bash
pip install pandas openpyxl
