# HR Attrition & Workforce Analytics Dashboard

## Project Overview

The **HR Attrition & Workforce Analytics Dashboard** is an interactive Power BI project designed to analyze employee workforce metrics and identify factors influencing employee attrition.

This dashboard helps HR teams and business stakeholders understand workforce distribution, salary structure, job roles, and key factors contributing to employee turnover. The analysis provides insights that can help organizations improve employee retention and workforce planning.

The project uses a **dimensional data model with fact and dimension tables**, enabling efficient analytics and scalable reporting.

---

## Business Problem

Employee attrition is a critical issue for organizations. High attrition can lead to:

* Increased recruitment costs
* Loss of experienced employees
* Reduced productivity
* Lower team morale

This dashboard aims to analyze workforce data and answer important business questions such as:

* Which departments have the highest attrition?
* Does overtime influence employee turnover?
* Does work-life balance affect employee retention?
* Which job roles contribute the most to payroll costs?
* What is the overall workforce structure of the organization?

---

## Dataset Description

The dataset represents **employee workforce data** containing information about employees, their job roles, performance metrics, satisfaction levels, and attrition status.

The project follows a **dimensional (star-style) data model** consisting of a fact table and multiple dimension tables.

### Fact Table

**Fact_Attrition**

This table stores employee attrition and workforce metrics.

Columns include:

* Employee_ID
* Attrition_Status
* JobSatisfaction
* Monthly_Income
* OverTime
* YearsAtCompany
* YearsSinceLastPromotion

---

### Dimension Tables

**Dim_Employee**

Contains employee demographic and job information.

Columns include:

* Employee_ID
* FullName
* Department
* Job_Role
* Age
* Gender
* Education_Level
* Experience_Years
* Marital_Status
* Salary

---

**Dim_Date**

Used for time-based analysis.

Columns include:

* Date
* Day
* Month
* Quarter
* Year

---

**Dim_Performance**

Stores employee performance metrics.

Columns include:

* Employee_ID
* Performance_Rating
* Manager_Feedback
* Last_Promotion_Year

---

**Dim_Satisfaction**

Stores employee satisfaction indicators.

Columns include:

* Employee_ID
* Environment_Satisfaction
* Job_Involvement
* Relationship_Satisfaction
* Work_Life_Balance

---

## Data Model

The dashboard is built using a **dimensional data model**.

Relationships:

Dim_Employee (1) ---- (*) Fact_Attrition
Dim_Date (1) -------- (*) Fact_Attrition
Dim_Performance (1) - (*) Dim_Employee
Dim_Satisfaction (1) - (*) Dim_Employee

This structure allows efficient filtering and interactive analysis across employee attributes.

---

## Dashboard Structure

The Power BI report contains **two main pages**.

### Page 1: HR Workforce Overview

This page provides a high-level overview of the workforce.

**Key KPIs**

* Total Employees
* Total Attrition
* Attrition Rate
* Average Salary
* Average Performance Rating

**Visualizations**

* Total Salary by Department
* Total Salary by Job Role
* Monthly Income by Years Since Last Promotion
* Department Filters
* Job Role Filters

This page helps stakeholders understand workforce distribution and salary structure.

---

### Page 2: Employee Attrition Analysis

This page focuses on identifying **factors influencing employee attrition**.

**KPIs**

* Total Attrition
* Attrition Rate
* Average Years at Company

**Visualizations**

* Attrition by Department
* Attrition by Work-Life Balance
* Attrition by Overtime
* Attrition by Performance Rating
* Department Filters
* Job Role Filters

This page helps analyze possible reasons behind employee turnover.

---

## Key Insights

Some insights that can be derived from the dashboard include:

* Departments experiencing employee turnover
* Impact of overtime on attrition
* Relationship between work-life balance and attrition
* Salary distribution across departments and job roles
* Performance trends across the workforce

These insights can help HR teams develop strategies to improve employee retention.

---

## Tools & Technologies Used

* Power BI Desktop
* DAX (Data Analysis Expressions)
* Dimensional Data Modeling
* Data Visualization

---

## Skills Demonstrated

This project demonstrates the following data analytics skills:

* Data Modeling (Fact and Dimension Tables)
* DAX Measures
* KPI Design
* Interactive Dashboard Development
* Business Intelligence Reporting
* HR Data Analysis

---

## Author

**Akshit Gajera**

Aspiring Data Analyst / Data Scientist skilled in:

* Python
* Machine Learning
* SQL
* Power BI
* Data Visualization

GitHub:
https://github.com/akshitgajera1013

---

## How to Use

1. Download the `.pbix` file from the repository.
2. Open it in **Power BI Desktop**.
3. Use filters and slicers to explore workforce and attrition insights.

---

## Project Purpose

This project was created as part of a **data analytics portfolio** to demonstrate Power BI dashboard development and business intelligence analysis using HR workforce data.
