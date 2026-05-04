# 📊 SQL Data Cleaning Project – Layoffs Dataset

## 📌 Overview

This project focuses on cleaning and preparing a real-world layoffs dataset using SQL. The goal is to transform raw data into a structured and analysis-ready format.

Dataset source: Kaggle Layoffs Dataset

---

## 🛠️ Tools Used

* SQL (MySQL)
* Window Functions
* Joins
* Data Cleaning Techniques

---

## 📂 Dataset

* Source: Kaggle
* Table Name: `layoffs`

---

## 🔧 Data Cleaning Steps

### 1. Remove Duplicates

* Used `ROW_NUMBER()` window function
* Identified duplicate rows based on all key columns
* Removed rows where `row_num > 1`

---

### 2. Standardize Data

* Replaced blank values with NULL
* Standardized industry names (e.g., Crypto variations)
* Cleaned country names (removed trailing periods)
* Converted date format using `STR_TO_DATE`

---

### 3. Handle Null Values

* Retained NULLs for meaningful analysis
* Populated missing industries using self join

---

### 4. Remove Unnecessary Data

* Deleted rows where both `total_laid_off` and `percentage_laid_off` were NULL
* Dropped helper column (`row_num`)

---

## 📈 Key Skills Demonstrated

* Data Cleaning in SQL
* Window Functions
* Data Standardization
* Query Optimization
* Real-world dataset handling

---

