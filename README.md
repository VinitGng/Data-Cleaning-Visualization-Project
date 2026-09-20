# Data Cleaning & Visualization Project

## 📌 Project Overview

This project focuses on cleaning, preprocessing, analyzing, and visualizing an employee dataset using Python.

The raw dataset was inspected for missing values, duplicate records, inconsistent text formatting, incorrect data types, and potential salary outliers. After cleaning, the processed dataset was analyzed using visualizations to understand employee distribution, age, and salary patterns.

## 🎯 Objectives

- Load and inspect a raw dataset
- Identify missing values
- Handle missing numerical values
- Remove duplicate records
- Clean text data
- Validate data types
- Detect potential outliers using the IQR method
- Create meaningful visualizations
- Export the cleaned dataset

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- OpenPyXL

## 📊 Dataset

The dataset contains employee information with the following fields:

- **Name** – Employee name
- **Age** – Employee age
- **Salary** – Employee salary
- **Join_Date** – Employee joining date
- **Department** – Employee department

## 🧹 Data Cleaning Process

### 1. Missing Values

Missing values were identified using Pandas.

- Age: 4 missing values
- Salary: 7 missing values

Missing Age and Salary values were filled using their respective median values.

### 2. Duplicate Records

One duplicate employee record was identified and removed.

The dataset was reduced from **43 rows to 42 rows**.

### 3. Text Cleaning

Leading and trailing whitespace was removed from text columns such as Name and Department.

### 4. Data Type Validation

The following data types were verified:

- Name → String
- Age → Numeric
- Salary → Numeric
- Join_Date → Datetime
- Department → String

### 5. Outlier Detection

Potential salary outliers were detected using the **Interquartile Range (IQR)** method.

The calculated upper bound was:

**98,802.50**

Six salary records were flagged as potential outliers.

These values were flagged rather than automatically deleted because a statistical outlier is not necessarily an incorrect value.

## 📈 Visualizations

The project includes:

- Employee count by department
- Salary distribution
- Age distribution
- Salary boxplot for outlier detection

## 📋 Final Dataset

After cleaning:

- **Rows:** 42
- **Columns:** 6
- **Missing values:** 0
- **Duplicate rows:** 0
- **Potential salary outliers:** 6

An additional `Salary_Outlier` column was created to identify potential salary outliers.


## 📁 Project Files

- `Data_Cleaning_Project.ipynb` – Jupyter Notebook containing the complete analysis
- `cleaned_employee_data.xlsx` – Cleaned Excel dataset
- `README.md` – Project documentation

## ✅ Conclusion

The project demonstrates a complete basic data-cleaning and visualization workflow using Python. The dataset was inspected, cleaned, validated, analyzed, and visualized. Potential salary outliers were identified using a statistical method while preserving the original salary values for further review.
