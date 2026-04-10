# 📊 Layoffs Data Analysis Project (SQL)

An end-to-end data cleaning and exploratory data analysis (EDA) project using SQL to analyze global layoffs trends.

---

## 🚀 Project Overview

This project focuses on **data cleaning** and **exploratory data analysis** of layoffs data from various companies worldwide. The goal is to prepare raw data for analysis and uncover meaningful insights about layoff patterns.

---

## 🎯 Project Objectives

- Clean and standardize raw layoffs data
- Remove duplicates and handle null values
- Perform exploratory data analysis (EDA)
- Identify key trends and patterns

---

## 🧰 Tech Stack

| Tool | Purpose |
|------|---------|
| **MySQL** | Data Cleaning & Analysis |
| **SQL** | Querying & Transformation |

---

## 📁 Dataset

Layoffs data including:
- Company names & locations
- Industries & stages
- Total & percentage laid off
- Dates & countries
- Funds raised

---

## 🧹 Data Cleaning Steps Performed

1. **Removed Duplicates** using `ROW_NUMBER()` with PARTITION BY
2. **Standardized Data**:
   - Trimmed company names
   - Fixed industry names (e.g., Crypto)
   - Removed dots from country names (e.g., United States)
3. **Date Formatting**:
   - Converted text dates to DATE format using `STR_TO_DATE()`
4. **Handled Null Values**:
   - Replaced blank industries with NULL
   - Populated missing industries using self-join
   - Removed rows where both `total_laid_off` and `percentage_laid_off` were NULL
5. **Dropped unnecessary columns** (e.g., `row_num`)

---

## 📈 Exploratory Data Analysis (EDA) Queries

| Analysis | Description |
|----------|-------------|
| Max Layoffs | Highest total and percentage laid off |
| Full Layoffs | Companies with 100% layoffs |
| By Stage | Total layoffs per company stage |
| By Year | Year-over-year layoff trends |
| Rolling Total | Monthly layoffs with cumulative sum |
| Top Companies | Companies with most layoffs |
| Yearly Ranking | Top 5 companies by layoffs per year |

---

## 🔍 Key SQL Techniques Used

- ✅ Common Table Expressions (CTEs)
- ✅ Window Functions (`ROW_NUMBER()`, `DENSE_RANK()`, `SUM() OVER()`)
- ✅ Self-Joins for data population
- ✅ String functions (`TRIM`, `SUBSTRING`)
- ✅ Date functions (`YEAR`, `STR_TO_DATE`)
- ✅ Aggregate functions (`SUM`, `MAX`, `MIN`)

---

## 📊 Sample Insights (from EDA)

- Highest layoffs occurred in specific years
- Certain industries/stages were hit harder
- Rolling totals show monthly accumulation trends
- Top 5 companies per year with maximum layoffs

---

## 🏗 Project Structure
-     layoffs_raw.csv

-     data_cleaning.sql

-     exploratory_analysis.sql

-     README.md



---

## 🧠 What I Learned

- Importance of data cleaning before analysis
- Real-world SQL techniques for messy data
- How to structure EDA for actionable insights
- Using window functions for advanced analytics

---

## ⭐ Future Improvements

- [ ] Visualize insights in Power BI / Tableau
- [ ] Add Python script for automated cleaning
- [ ] Compare layoffs across economic cycles

---

## 📫 Connect

Feel free to use this project for your portfolio!

---

⭐ **Don't forget to star this project if you found it helpful!** ⭐
