# 📊 Employee Attrition Analysis Dashboard (Power BI)

---

# 1. Project Overview

This project focuses on analyzing **employee attrition** using Power BI.

**Employee Attrition** refers to the number of employees who leave an organization over a period of time due to resignation, termination, retirement, or other reasons.

This dashboard helps HR teams understand:

* Why employees are leaving
* Which groups are most affected
* What factors influence attrition

---

# 2. Objective of the Project

The main objectives are:

* Identify key drivers of attrition
* Analyze employee behavior patterns
* Compare attrition across departments and job roles
* Provide interactive insights using filters
* Support HR decision-making

---

# 3. Why This Dashboard is Important

Employee attrition is a major concern because:

* High attrition increases hiring costs
* Impacts productivity and team stability
* Causes knowledge loss
* Reduces company performance

> This dashboard helps organizations:

* Reduce employee turnover
* Improve job satisfaction
* Take preventive actions

---

# 4. When is This Used?

This dashboard is used:

* During HR review meetings
* While analyzing employee retention
* Before planning hiring strategies
* To identify high-risk employees
* For performance and satisfaction analysis

---

# 5. Dataset Information

* Dataset Name: **Employee Attrition Dataset**
* Total Records: ~9800 employees
* Type: HR structured dataset

### Key Features (Columns):

* Age
* Gender
* Department
* Job Role
* Monthly Income
* Job Satisfaction (1–5 scale)
* Work Environment Satisfaction
* Work Life Balance
* Overtime (Yes/No)
* Years at Company
* Distance From Home
* Performance Rating
* Attrition (Yes/No)

---

# 6. Data Cleaning Process (VERY IMPORTANT)

Data cleaning was done using Power BI (Power Query).

### ✔ Step-by-step cleaning:

#### 1. Handling Inconsistent Values

* Converted values like:

  * `yes`, `YES`, `Yes` → **Yes**
  * `no`, `No` → **No**

#### 2. Removed Duplicates

* Checked for duplicate employee records
* Ensured each employee is unique

#### 3. Handled Missing Values

* Checked null values in columns
* Replaced or removed where necessary

#### 4. Corrected Data Types

* Age → Whole Number
* Income → Numeric
* Attrition → Categorical

#### 5. Created Calculated Measures

**Attrition Count**

```DAX
Attrition Count = COUNTROWS(FILTER(Table, Table[Attrition] = "Yes"))
```

**Attrition Rate**

```DAX
Attrition Rate = DIVIDE([Attrition Count], COUNT(Table[Employee_ID]))
```

#### 6. Created Bins (Grouping)

* Age → grouped into ranges
* Monthly Income → grouped
* Years at Company → grouped

---

# 7. Dashboard Features

##  KPI Cards

* Total Employees → 9800
* Attrition Rate → 49.19%
* Attrition Count → 1997

---

# 8. Visualizations Used

## 1. Bar Chart

Used for:

* Attrition by Department
* Attrition by Job Role

---

## 2. Column Chart

Used for:

* Job Satisfaction vs Attrition
* Work Life Balance vs Attrition

---

## 3. Pie / Donut Chart

Used for:

* Attrition by Gender
* Attrition by Marital Status

---

## 4. Line Chart

Used for:

* Years at Company vs Attrition

---

## 5. Clustered Chart

Used for:

* Age vs Attrition by Gender

---

## 6. Table

Used for:

* Work Environment Satisfaction summary

---

# 9. Filters (Slicers)

The dashboard includes interactive slicers:

* Department
* Job Role
* Gender
* Overtime
* Job Satisfaction

---

# 10. What This Dashboard Visualizes

The dashboard provides insights into:

* Which departments have high attrition
* Which job roles are most affected
* Impact of job satisfaction on attrition
* Relationship between overtime and attrition
* Gender-based attrition distribution
* Employee behavior based on experience

---

# 11. Key Insights

* Employees with **low job satisfaction** have higher attrition
* **Overtime workers** tend to leave more
* Certain **job roles and departments** show higher attrition
* Attrition varies across **age groups and experience levels**

---

# 🛠 12. Tools & Technologies Used

* Power BI
* Power Query
* DAX (Data Analysis Expressions)
* Data Visualization Techniques

---

# 13. Project Files

* Employee_Attrition_Dashboard.pbix
* Dashboard Screenshot
* README.md

---

# 14. Conclusion

This dashboard helps organizations:

* Identify attrition patterns
* Improve employee satisfaction
* Reduce turnover
* Make better HR decisions

---

# 15. Future Improvements

* Add predictive analysis (ML)
* Include salary benchmarking
* Add employee feedback analysis
* Connect with live database

---

# Author
**Chandana KS**
BCA Student | Data Analytics Enthusiast
