# employee-dataset
This project uses a synthetic employee dataset containing employee demographics, department information, salary, and joining date. The raw dataset contains inconsistent formatting and missing standardization, making it suitable for demonstrating Excel data cleaning techniques.

Dataset Link: https://docs.google.com/spreadsheets/d/1xMxtRGwnAEdz4RwS2Rvr6hGsQqfJlDKQC2jf_lsh4MU/edit?usp=sharing

### Raw Dataset Preview

| Employee ID | First Name | Last Name | Age | Gender | Department | Phone | Salary | Joined |
|--------------|------------|-----------|----:|--------|------------|--------|---------|---------|
| emp1000 | Alya | Utami | 39 | f | FINANCE | 0898-597 2064 | 10695230 | 18/03/2022 |
| emp1001 | nanda | Utami | 52 | M | hr | 08951307245 | Rp 11920261 | 2022-08-21 |
| emp1002 | lina | permata | 35 | mAle | hr | 08890573997 | 12373985 | 21/06/2021 |
| emp1003 | bima | Nugroho | 34 | mAle | Marketing | 08155050949 | Rp 14631304 | 2022-07-18 |
| emp1004 | tio | Putra | 24 | mAle | CustomerSupport | 08447327900 | 17015532 | 03/12/2020 |
| emp1005 | eka | Andini | 37 | male | It | 08833570085 | 9326818 | 2020-08-18 |
| emp1006 | Fajar | sari | 53 | mAle | FINANCE | 08519222403 | 7150189 | 06/10/2019 |
| emp1007 | Dimas | Wijaya | 39 | male | CustomerSupport | 0864-518 6885 | 14306122 | 2024-07-10 |

---

### Cleaned Dataset Preview

| Employee ID | Full Name | Age | Age Group | Gender | Department | Salary | Year Joined |
|--------------|-----------|----:|-----------|--------|------------|---------|------------:|
| EMP1000 | Alya Utami | 39 | Junior | Female | Finance | Rp10.695.230 | 2022 |
| EMP1001 | Nanda Utami | 52 | Senior | Male | HR | Rp11.920.261 | 2022 |
| EMP1002 | Lina Permata | 35 | Junior | Male | HR | Rp12.373.985 | 2021 |
| EMP1003 | Bima Nugroho | 34 | Junior | Male | Marketing | Rp14.631.304 | 2022 |
| EMP1004 | Tio Putra | 24 | Junior | Male | Customer Support | Rp17.015.532 | 2020 |
| EMP1005 | Eka Andini | 37 | Junior | Male | IT | Rp9.326.818 | 2020 |
| EMP1006 | Fajar Sari | 53 | Senior | Male | Finance | Rp7.150.189 | 2019 |
| EMP1007 | Dimas Wijaya | 39 | Junior | Male | Customer Support | Rp14.306.122 | 2024 |

## Data Cleaning

Several data cleaning techniques were applied to improve data quality.

### Data Cleaning Tasks

- Combined first name and last name into **Full Name** with **CONCATENATE**
- Standardized name formatting using **PROPER()**
- Cleaned phone numbers using **REGEXREPLACE()**
- Removed currency symbols from salary values
- Converted salary into Currency format
- Converted joining dates into Date format
- Standardized gender values using **IF()**
- Converted inconsistent age values using **SWITCH()**
- Standardized department names using **SWITCH()**
- Created **Age Group** classification (Junior / Senior)
- Added filters for easier data exploration

---

## Excel Functions Used

- CONCATENATE()
- PROPER()
- REGEXREPLACE()
- IF()
- SWITCH()
- VALUE()
- TRIM()
- UPPER()
- LOWER()
- VLOOKUP()

---

## Pivot Tables

The project includes Pivot Tables to analyze:

- Employee distribution by department
- Gender distribution within each department
- Joining year by department
- Total salary for each department

---

## Dashboard

![Dashboard](dashboard-employee)

The interactive dashboard includes:

### KPI Cards

- Total Employees
- Total Salary
- Average Salary

### Visualizations

- Salary by Department
- Employee Distribution by Department
- Salary Trend by Joining Year
- Gender Distribution
- Age Group Distribution

### Interactive Filters

- Department
- Gender
- Age Group

---

## VLOOKUP Practice

A separate worksheet demonstrates the use of **VLOOKUP**.

Using **Employee ID** as the lookup value, the project automatically retrieves:

- Assigned Employee Name
- Department

from the employee master dataset.

---

## Skills Demonstrated

- Data Cleaning
- Data Transformation
- Excel Functions
- VLOOKUP
- Pivot Tables
- Dashboard Design
- KPI Reporting
- Data Visualization
