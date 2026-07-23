# 🏦 Apex Bank HR Workforce Analytics Dashboard

> **An End-to-End Business Intelligence Solution for Workforce Analytics, HR Performance Monitoring, and Executive Decision Support using Microsoft Power BI.**

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-Data%20Analysis-blue?style=for-the-badge)
![Power Query](https://img.shields.io/badge/Power%20Query-Transformation-success?style=for-the-badge)
![Business Intelligence](https://img.shields.io/badge/Business-Intelligence-orange?style=for-the-badge)
![HR Analytics](https://img.shields.io/badge/HR-Analytics-red?style=for-the-badge)

---

# 📸 Dashboard Preview

## Executive HR Dashboard

![Executive Dashboard](images/apex_dashboard.png)

---

## Workforce Analytics Dashboard

![Workforce Dashboard](images/workflow_details.png)

---

## Data Quality Dashboard

![Data Quality Dashboard](images/data_quality.png)

---

# 📖 Executive Summary

Human Resources is more than managing employee records—it is responsible for making strategic decisions that directly influence organizational performance, employee satisfaction, productivity, and long-term business growth. These decisions depend on accurate, reliable, and accessible data.

In many organizations, HR data is collected from multiple operational systems and maintained over time by different users. As a result, datasets often contain inconsistent department names, duplicate records, missing values, incorrect salary formats, mixed date formats, and other data quality issues that reduce the reliability of business reports.

This project demonstrates how these challenges can be addressed through Business Intelligence.

Using Microsoft Power BI, Power Query, and DAX, a complete HR analytics solution was developed for **Apex Bank Plc**, transforming raw employee records into an interactive executive dashboard that supports workforce planning, performance monitoring, salary analysis, employee retention, leave management, and data quality reporting.

Rather than presenting raw figures, the dashboard converts HR data into meaningful business insights, enabling management to monitor workforce trends, evaluate organizational performance, identify operational risks, and make evidence-based decisions with confidence.

---

# 💼 Business Challenge

Human Resources departments generate thousands of employee records throughout an organization's lifecycle. While these records contain valuable information, they often become difficult to analyze because of inconsistent data entry, duplicate records, formatting issues, and missing information.

For Apex Bank, these data quality challenges reduced confidence in HR reporting and limited management's ability to answer important workforce questions such as:

- How many employees are currently active?
- Which departments employ the largest workforce?
- Which grade levels receive the highest compensation?
- What is the current employee attrition rate?
- Which departments experience the highest employee turnover?
- How long do employees typically remain with the organization?
- Are employees fully utilizing their annual leave entitlement?
- How reliable is the available HR data?

Without accurate reporting, HR leaders risk making strategic decisions based on incomplete or misleading information.

This project addresses these challenges by transforming raw HR data into an interactive Business Intelligence solution that delivers reliable insights through automated reporting and executive dashboards.

---

# 🎯 Project Objectives

The primary objective of this project was to design a professional HR analytics dashboard capable of supporting executive decision-making through clean, validated, and interactive reporting.

### Business Objectives

- Monitor the overall workforce size.
- Track active and exited employees.
- Analyze workforce distribution across departments and grade levels.
- Evaluate gender diversity within the organization.
- Compare salary distribution across grade levels.
- Measure employee performance across departments.
- Evaluate employee tenure and retention.
- Monitor annual leave utilization.
- Assess the quality of HR data before analysis.

### Technical Objectives

- Clean and transform raw HR data using Power Query.
- Resolve data quality issues affecting reporting accuracy.
- Build reusable DAX measures for business KPIs.
- Design an optimized analytical data model.
- Develop an interactive executive dashboard using Power BI.
- Present business insights through effective data storytelling.

---

# 🏦 Business Understanding

This dashboard was designed to support different stakeholders across Apex Bank, each with unique information requirements.

| Stakeholder | Business Need |
|------------|---------------|
| Executive Management | Monitor workforce health and strategic HR performance |
| Human Resources Department | Track employee performance, retention, and workforce planning |
| Department Managers | Monitor departmental staffing and employee productivity |
| Finance Department | Analyze salary distribution and payroll trends |
| Business Executives | Make data-driven workforce decisions |

The dashboard serves as a centralized decision-support solution by combining multiple HR metrics into a single interactive reporting environment.

---

# 📂 Dataset Overview

**Organization:** Apex Bank Plc *(Fictional)*

**Industry:** Banking

**Business Function:** Human Resources

**Visualization Tool:** Microsoft Power BI

**Data Preparation:** Power Query

**Business Calculations:** DAX (Data Analysis Expressions)

**Dataset Size:** Approximately **2,080 employee records**

The dataset contains employee-level information covering workforce demographics, organizational structure, compensation, employment history, performance evaluation, annual leave usage, and employee status.

Key business entities represented within the dataset include:

- Employee Information
- Department
- Grade Level
- Gender
- Employment Type
- Gross Salary
- Date of Joining
- Exit Date
- Employee Status
- Performance Rating
- Annual Leave Days Used
- Contact Information

Together, these attributes provide the foundation for analyzing workforce composition, employee retention, compensation trends, departmental performance, and overall HR effectiveness.

---

# 🔄 Project Workflow

This project followed a structured Business Intelligence workflow to transform raw HR data into meaningful insights that support strategic decision-making at Apex Bank.

```
Business Understanding
        │
        ▼
Data Collection
        │
        ▼
Data Profiling
        │
        ▼
Data Cleaning & Transformation
        │
        ▼
Data Validation
        │
        ▼
Data Modeling
        │
        ▼
DAX Measure Development
        │
        ▼
Dashboard Design
        │
        ▼
Business Insight Generation
        │
        ▼
Executive Decision Support
```

Each stage of the workflow was carefully executed to ensure that the final dashboard was built on accurate, reliable, and business-ready data.

---

# 🧹 Data Cleaning & Transformation

Before building the dashboard, the raw HR dataset was thoroughly assessed to identify issues that could compromise reporting accuracy. Data preparation was performed entirely in **Power Query**, ensuring consistency across all analyses and visualizations.

> 📷 **Insert your Power Query Editor Screenshot here**

## Data Quality Issues Identified

The original dataset contained several data quality issues, including:

- Duplicate employee records
- Inconsistent department naming
- Invalid Gross Salary values
- Negative salary amounts
- Mixed date formats
- Missing values
- Inconsistent Gender values
- Inconsistent Marital Status values
- Inconsistent Employment Type values
- Invalid email addresses
- Incorrect phone number formats
- Exit Date and Employee Status inconsistencies
- Annual Leave values exceeding company policy
- Invalid Performance Ratings

Without resolving these issues, KPIs such as Attrition Rate, Average Salary, Employee Tenure, and Department Headcount would produce misleading results.

---

# ⚙️ Power Query Transformations

The following transformations were performed to improve the quality and reliability of the dataset.

| Transformation | Purpose |
|---------------|---------|
| Removed duplicate records | Eliminated duplicate employee entries to avoid inflated headcount. |
| Standardized Department names | Ensured departments such as "Finance" and "Finance & Account" were reported consistently. |
| Corrected Gross Salary values | Removed invalid characters, converted salaries to numeric values, and corrected negative salaries using `Number.Abs()`. |
| Standardized Gender values | Unified inconsistent entries such as Male, male, M, Female, female, and F. |
| Standardized Marital Status | Corrected inconsistent text values for reliable demographic reporting. |
| Standardized Employment Type | Unified employment categories across the dataset. |
| Converted Date columns | Converted mixed date formats into a consistent Date data type. |
| Trimmed unnecessary spaces | Removed leading and trailing spaces from text fields. |
| Corrected Email formatting | Improved consistency of employee email records. |
| Standardized Phone Numbers | Corrected formatting inconsistencies and invalid lengths. |
| Validated Exit Dates | Ensured Exit Date aligned logically with Employee Status. |
| Reviewed Leave Values | Identified leave records exceeding the organization's annual leave policy. |
| Validated Performance Ratings | Identified ratings outside the expected business range. |

These transformations significantly improved data quality and ensured that every KPI displayed within the dashboard was based on clean, validated information.

---

# 📋 Data Quality Summary

> 📷 **Insert your Data Quality Dashboard Screenshot here**

To improve transparency and increase confidence in the final analysis, a dedicated Data Quality Dashboard was developed to summarize the issues identified during data preparation.

The dashboard documents the number of records affected by each issue, the percentage of the dataset impacted, and the corrective action taken before analysis.

This approach demonstrates that the business insights presented throughout the report are based on trusted, validated data rather than raw operational records.

Key improvements included:

- Standardizing inconsistent categorical values.
- Correcting salary anomalies.
- Resolving formatting inconsistencies.
- Validating employee status information.
- Improving data completeness.
- Enhancing reporting accuracy.

Including a dedicated Data Quality report reinforces an important Business Intelligence principle:

> **Reliable business decisions begin with reliable data.**

---

# 🗂️ Data Model

> 📷 **Insert your Model View Screenshot here**

A structured data model was developed to support efficient calculations and interactive reporting within Power BI.

The model was designed to:

- Improve dashboard performance.
- Ensure accurate DAX calculations.
- Maintain consistent filtering across visuals.
- Simplify report maintenance.
- Support future scalability.

A well-structured model reduces redundancy and enables users to explore HR data dynamically across departments, grade levels, employment types, and employee demographics.

---

# 📐 DAX Measures Developed

Several DAX measures were created to answer the business questions defined for this project.

| Measure | Business Purpose |
|---------|------------------|
| Total Employees | Calculates the total workforce. |
| Active Employees | Counts employees currently employed. |
| Total Exited Employees | Counts employees with a recorded Exit Date. |
| Attrition Rate (%) | Measures employee turnover as a percentage of the workforce. |
| Average Gross Salary | Calculates the average employee salary. |
| Average Performance Rating | Measures overall workforce performance. |
| Average Employee Tenure | Calculates the average years employees have worked. |
| Employees Used Full Leave | Counts employees who utilized their full annual leave entitlement. |
| Full Leave Utilization (%) | Calculates leave utilization across the workforce. |
| Female Percentage by Department | Measures female representation within departments. |
| Employees Rated 1 or 2 | Identifies low-performing employees. |
| Headcount by Department | Measures workforce distribution across departments. |
| Headcount by Grade Level | Measures workforce distribution across grade levels. |

These measures transformed raw employee records into meaningful business metrics that support strategic HR reporting.
