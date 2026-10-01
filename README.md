# IBM HR Analytics – Employee Attrition EDA

## 📌 Project Overview

This project performs Exploratory Data Analysis (EDA) on the **IBM HR Analytics Employee Attrition & Performance** dataset.

The main objective is to understand employee attrition patterns and identify factors that are associated with employees leaving the organization.

The analysis investigates factors such as:

- Department
- Overtime
- Monthly Income
- Job Satisfaction
- Distance From Home
- Job Role
- Age
- Work-Life Balance
- Employee experience and other workforce characteristics

---

## 🎯 Objectives

The project answers the following questions:

1. What is the overall attrition rate?
2. Which departments have higher attrition?
3. Does overtime relate to attrition?
4. Does salary/income differ between employees who leave and stay?
5. How does job satisfaction relate to attrition?
6. Does distance from home have any relationship with attrition?
7. Which job roles have higher attrition?
8. Does age influence attrition patterns?
9. How does work-life balance relate to employee retention?
10. What differences can be observed between employees who left and those who stayed?

---

## 📊 Dataset

**Dataset:** IBM HR Analytics Employee Attrition & Performance

**Number of records:** 1,470 employees

**Original number of columns:** 35

After data cleaning, 32 relevant columns were retained.

The dataset contains employee information related to:

- Demographics
- Job roles
- Department
- Monthly income
- Job satisfaction
- Work-life balance
- Overtime
- Distance from home
- Years of experience
- Attrition

---

## 🧹 Data Cleaning

The following data-cleaning steps were performed:

- Checked the dataset dimensions.
- Inspected data types and column information.
- Checked for missing values.
- Checked for duplicate records.
- Examined unique values and categorical variables.
- Identified constant columns.
- Removed columns that contained no useful variation:
  - `Over18`
  - `StandardHours`
  - `EmployeeCount`
- Identified `EmployeeNumber` as an employee identifier and excluded it from analytical interpretation.
- Checked numerical variables for potential outliers using the IQR method.
- Plausible outliers were retained because they represented realistic employee/workplace values.

### Missing Values

There were **no missing values** in the dataset.

### Duplicate Records

There were **no duplicate records**.

---

## 🔍 Exploratory Data Analysis

### 1. Overall Attrition Rate

The dataset contains:

- Employees who stayed: **1,233**
- Employees who left: **237**

The overall attrition rate is:

**16.12%**

---

### 2. Attrition by Department

Observed attrition rates:

| Department | Attrition Rate |
|---|---:|
| Human Resources | 19.05% |
| Research & Development | 13.84% |
| Sales | 20.63% |

The observed attrition rate varies across departments.

---

### 3. Overtime and Attrition

Observed attrition rates:

| Overtime | Attrition Rate |
|---|---:|
| No | 10.44% |
| Yes | 30.53% |

Employees working overtime had a higher observed attrition rate than employees who did not work overtime.

This indicates an association between overtime and attrition in this dataset; it does not establish causation.

---

### 4. Monthly Income and Attrition

| Attrition | Mean Monthly Income | Median Monthly Income |
|---|---:|---:|
| No | 6,832.74 | 5,204 |
| Yes | 4,787.09 | 3,202 |

Employees who stayed had higher average and median monthly income than employees who left.

---

### 5. Job Satisfaction and Attrition

Observed attrition rates:

| Job Satisfaction Level | Attrition Rate |
|---|---:|
| 1 | 22.84% |
| 2 | 16.43% |
| 3 | 16.52% |
| 4 | 11.33% |

Lower job satisfaction levels show higher observed attrition rates in the dataset.

---

### 6. Distance From Home and Attrition

| Attrition | Mean Distance From Home | Median |
|---|---:|---:|
| No | 8.92 | 7 |
| Yes | 10.63 | 9 |

Employees who left had a higher average and median distance from home compared with employees who stayed.

---

### 7. Attrition by Job Role

Observed attrition rates:

| Job Role | Attrition Rate |
|---|---:|
| Sales Representative | 39.76% |
| Laboratory Technician | 23.94% |
| Human Resources | 23.08% |
| Sales Executive | 17.48% |
| Research Scientist | 16.10% |
| Manufacturing Director | 6.90% |
| Healthcare Representative | 6.87% |
| Manager | 4.90% |
| Research Director | 2.50% |

Attrition rates vary considerably across job roles.

---

### 8. Age and Attrition

Employees were grouped into four age groups.

| Age Group | Attrition Rate |
|---|---:|
| 18–25 | 35.77% |
| 26–35 | 19.14% |
| 36–45 | 9.19% |
| 46–60 | 12.45% |

The 18–25 age group has the highest observed attrition rate, while the 36–45 group has the lowest.

The relationship is not perfectly linear because the 46–60 group shows a slight increase compared with the 36–45 group.

---

### 9. Work-Life Balance and Attrition

Observed attrition rates:

| Work-Life Balance Level | Attrition Rate |
|---|---:|
| 1 | 31.25% |
| 2 | 16.86% |
| 3 | 14.22% |
| 4 | 17.65% |

Employees with the lowest work-life balance level show the highest observed attrition rate.

The relationship is not strictly linear because level 4 has a slightly higher attrition rate than level 3.

---

## 📈 Visualizations

The project uses visualizations to understand the relationships between employee characteristics and attrition.

Visualizations include:

- Attrition distribution
- Department-wise attrition
- Overtime vs attrition
- Monthly income comparison
- Job satisfaction vs attrition
- Distance from home comparison
- Job role-wise attrition
- Age group vs attrition
- Work-life balance vs attrition

---

## 🛠️ Technologies Used

- **Python**
- **Jupyter Notebook**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**

---

## 📂 Project Structure

```text
HR-Employee-Attrition-EDA/
│
├── Employee_Attrition_EDA.ipynb
├── WA_Fn-UseC_-HR-Employee-Attrition.csv
├── .gitignore
└── README.md
