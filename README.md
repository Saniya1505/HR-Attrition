# HR Attrition Analysis | Microsoft Fabric & Power BI

## 📌 Project Overview

**HR Attrition Analysis** is an end-to-end HR analytics project built using Microsoft Fabric and Power BI to analyze employee turnover, identify attrition patterns, and uncover workforce trends that can help organizations make data-driven HR decisions.

The project transforms HR data into an interactive, two-page dashboard that examines employee attrition across departments, job roles, salary bands, age groups, gender, education, marital status, business travel, and overtime.

The objective is to help HR teams understand **who is leaving, which employee groups have higher attrition rates, and which factors deserve further investigation.**

## 🎯 Business Objectives

- Measure overall employee attrition and workforce size.
- Identify departments and job roles with high employee turnover.
- Analyze attrition across salary bands and demographic groups.
- Examine relationships between overtime, business travel, and employee attrition.
- Compare employee headcount and attrition rates across different categories.
- Present HR metrics through an interactive dashboard to support workforce planning and retention strategies.

## 🛠️ Tools & Technologies

| Tool / Technology | Purpose |
|---|---|
| Microsoft Fabric | Data analytics workspace and project environment |
| Dataflow Gen2 | Data preparation and transformation |
| Microsoft Fabric Lakehouse | Data storage and data management |
| SQL Analytics Endpoint | SQL-based access to Lakehouse data |
| Semantic Model | Organizing data and defining relationships and analytical measures |
| Power BI | Interactive dashboard development and visualization |
| DAX | Calculating HR KPIs and attrition metrics |
| Power Query | Data cleaning and transformation through the dataflow |

## 🏗️ Project Architecture

The project follows a data analytics workflow that moves from data preparation to storage, modeling, and visualization.

**Workflow:**

Source HR Data → Data Preparation → Microsoft Fabric Lakehouse → Semantic Model → Power BI Report

### Architecture Components

1. **Data Preparation — Dataflow Gen2 (`Df_HR`)**

   Imported and prepared the HR dataset for analysis. This layer supports data cleaning and transformation before the data is used in reporting.

2. **Data Storage — Lakehouse (`lh_HR`)**

   Used Microsoft Fabric Lakehouse as the central storage layer for the prepared HR data.

3. **Data Access — SQL Analytics Endpoint**

   Provides SQL-based access to supported Lakehouse tables for querying and analysis.

4. **Data Modeling — Semantic Model (`Hr semantic`)**

   Organized the data for reporting and provided the model through which report visuals and analytical calculations interact with the underlying data.

5. **Data Visualization — Power BI Report (`HR Attrition Analysis`)**

   Built an interactive, two-page report with KPI cards, bar charts, tables, conditional formatting, slicers, and an attrition decomposition visual.

## 📊 Dashboard Pages

### 1. Overview

The Overview page provides a high-level summary of employee attrition and workforce composition.

**Key Performance Indicators (KPIs):**

- **Attrition Rate:** 16.1%
- **Employees Left:** 237
- **Total Headcount:** 1,470
- **Average Monthly Income:** 6,503
- **Average Tenure of Leavers:** 5.1 years

**Visualizations:**

- Attrition Rate by Department
- Attrition Decomposition by Department, Job Role, and Salary Band
- Attrition by Job Role, including headcount, employees who left, and attrition rate
- Attrition by Salary Band, including headcount, employees who left, and attrition rate
- Overall workforce split between employees who stayed and those who left

**Interactive Filters:**

- Department
- Gender
- Salary Band

These filters allow users to explore different employee groups and examine how attrition metrics change across the selected categories.

### 2. Deep Dive

The Deep Dive page explores attrition patterns across demographic, educational, and workplace-related categories.

**Visualizations:**

- Attrition by Age Group
- Attrition Rate by Gender
- Attrition by Education Field
- Attrition Rate by Marital Status
- Attrition Rate by Business Travel Frequency
- Attrition Rate by Overtime Status

This page helps identify employee segments with comparatively high attrition rates and provides additional context for HR investigations.

## 🔍 Key Insights

The dashboard highlights several patterns in the dataset:

- **Overall attrition:** 16.1% of the workforce, representing 237 employees, left the organization.
- **Department-level attrition:** Sales has the highest displayed attrition rate at 20.6%, followed by Human Resources at 19.0%.
- **Age groups:** Employees aged 18–25 have the highest displayed attrition rate at 35.8%.
- **Salary bands:** Employees earning under 3k have an attrition rate of 28.6%, compared with 8.9% for employees earning above 10k.
- **Overtime:** Employees working overtime have a displayed attrition rate of 30.5%, compared with 10.4% for employees not working overtime.
- **Business travel:** Employees who travel frequently have a displayed attrition rate of 24.9%, compared with 8.0% for non-travellers.
- **Job roles:** Sales Representatives have the highest displayed job-role attrition rate at 39.8%.
- **Education fields:** Human Resources has the highest displayed attrition rate among education fields at 25.9%.

These findings indicate employee groups that may warrant further investigation. The dashboard reveals associations in the dataset; it does not establish that any single factor directly causes employees to leave.

## ⚙️ Technical Implementation

The project brings together data preparation, storage, semantic modeling, and interactive reporting within Microsoft Fabric.

Key implementation areas include:

- Preparing HR data for analysis using Dataflow Gen2 and Power Query.
- Storing prepared data in a Fabric Lakehouse.
- Accessing Lakehouse data through the SQL Analytics Endpoint.
- Using a semantic model to support consistent reporting.
- Developing workforce KPIs and attrition calculations.
- Designing interactive report pages with slicers and cross-filtering.
- Using conditional formatting to highlight comparatively high and low attrition rates.
- Creating an attrition decomposition visual to investigate contributing categories.
- Presenting metrics through KPI cards, charts, and detailed tables.

## 🧠 Skills Demonstrated

**Data Analytics**
- Exploratory Data Analysis (EDA)
- HR Analytics and Workforce Analysis
- KPI Development and Monitoring
- Attrition Rate Analysis
- Comparative and Trend Analysis
- Business Insight Generation

**Data Engineering & Modeling**
- Data Preparation and Transformation
- Dataflow Gen2
- Lakehouse-Based Data Storage
- SQL Analytics Endpoint
- Semantic Modeling

**Business Intelligence**
- Power BI Dashboard Development
- DAX-Based Calculations
- Interactive Slicers and Filtering
- Data Visualization and Conditional Formatting
- Report Layout and Information Design

**Business Problem-Solving**
- Identifying High-Risk Employee Segments
- Translating Data into Business Insights
- Supporting Data-Driven Workforce Planning

## 💼 Business Value

This dashboard can help HR teams:

- Identify departments and roles that may require targeted retention strategies.
- Investigate turnover patterns across age groups and salary bands.
- Examine potential relationships between overtime, travel requirements, and attrition.
- Monitor workforce metrics in a centralized report.
- Prioritize further analysis of employee groups with elevated turnover.

The findings can guide further investigation into compensation, workload, career progression, employee engagement, and retention initiatives.

## 📸 Dashboard Preview

### Overview Page

<img width="1917" height="871" alt="Screenshot 2026-10-14 212246" src="https://github.com/user-attachments/assets/7bfd4fdf-d9ba-4c4d-8e6f-ea4d16f9a01a" />

### Deep Dive Page

<img width="1916" height="877" alt="Screenshot 2026-10-14 212306" src="https://github.com/user-attachments/assets/02503b53-74e9-49f9-bb26-ab606fa56572" />

*Note: Add the two dashboard screenshots to an `images` folder in your GitHub repository using the filenames shown above, or update the image paths to match your actual filenames.*

## 📁 Project Components

The project was developed in Microsoft Fabric and includes the following workspace items:

- `Df_HR` — Dataflow Gen2
- `lh_HR` — Lakehouse
- `lh_HR` — SQL Analytics Endpoint
- `Hr semantic` — Semantic Model
- `HR Attrition Analysis` — Power BI Report

<img width="1907" height="872" alt="Screenshot 2026-10-14 212116" src="https://github.com/user-attachments/assets/3a5d1207-fce5-4179-afb1-377a2e5112fc" />


## 🚀 Future Enhancements

- Add automated data refresh and monitoring.
- Develop an employee attrition prediction model using machine learning.
- Incorporate employee satisfaction, performance, and engagement metrics where available.
- Build a retention-risk scoring framework.
- Add time-based attrition trends if historical HR data becomes available.
- Document the data transformation logic and DAX measures in greater detail.

## 📚 Project Summary

This project demonstrates the use of Microsoft Fabric and Power BI to build an end-to-end HR analytics solution, from data preparation and storage to semantic modeling, KPI development, and interactive reporting.

It showcases practical skills in data analytics, business intelligence, data modeling, dashboard design, and translating workforce data into actionable business insights.

