# HR Attrition & Retention Analytics Dashboard

## Executive Summary

Employee attrition represents one of the most significant hidden costs to organizational performance, with replacement costs typically ranging from 50% to 200% of an employee's annual salary once recruitment, onboarding, and lost-productivity overhead are factored in. This project delivers an end-to-end **HR analytics solution** built in Excel, transforming raw workforce data into actionable, executive-ready insights on employee attrition and retention risk.

Using a dataset of **1,470 employee records across 35 HR attributes**, this analysis quantifies attrition drivers, segments high-risk employee cohorts, and surfaces the compensation, satisfaction, and tenure factors most strongly correlated with voluntary turnover — enabling HR leadership to move from reactive headcount reporting to **proactive, data-driven retention strategy**.

---

## Project Objectives

- Quantify the organization's current **attrition rate** and benchmark it against total headcount
- Identify the **key predictive variables** driving voluntary employee turnover (compensation, job satisfaction, overtime, tenure, work-life balance, etc.)
- Segment attrition risk across **department, job role, job level, and demographic dimensions**
- Translate raw HRIS-style data into a **self-service executive dashboard** for stakeholder decision-making
- Establish a repeatable analytical framework that can be refreshed as new workforce data becomes available

---

## Dataset Overview

| Attribute | Detail |                                                       <img width="1919" height="1079" alt="Screenshot 2026-07-01 122824" src="https://github.com/user-attachments/assets/839b43f3-7ed6-482e-8042-25b2c501c959" />

|---|---|
| **Total Records** | 1,470 employees |
| **Total Attributes** | 35 HR variables |
| **Leavers Identified** | 237 employees |
| **Overall Attrition Rate** | 16.1% |

**Key data dimensions captured include:**
- **Demographic & Employment Data:** Age, Gender, Marital Status, Education, Education Field
- **Compensation Metrics:** Monthly Income, Hourly Rate, Daily Rate, Monthly Rate, Percent Salary Hike, Stock Option Level
- **Engagement & Satisfaction Indices:** Job Satisfaction, Environment Satisfaction, Relationship Satisfaction, Job Involvement, Work-Life Balance
- **Career Progression Metrics:** Job Level, Job Role, Years at Company, Years in Current Role, Years Since Last Promotion, Years with Current Manager, Total Working Years
- **Operational Factors:** OverTime, Business Travel, Distance From Home, Number of Companies Worked, Training Times Last Year, Performance Rating

---
<img width="831" height="518" alt="Screenshot 2026-07-01 122327" src="https://github.com/user-attachments/assets/ca4ff7bf-ad9b-43d7-b7b3-afd82eb8f37a" />

## Methodology & Technical Approach

This project applies a structured **data-to-insight pipeline** using native Excel business intelligence capabilities:

1. **Data Ingestion & Structuring** — Raw HR records normalized into a tabular data model (`Raw_Data` sheet) with consistent field typing across all 35 variables.
2. **Data Modeling & Aggregation** — A dedicated `Calculations` layer leverages **PivotTables** to compute headcount, attrition counts, and attrition rate, alongside cross-tabulated breakdowns (e.g., average monthly income by job role, attrition by department, satisfaction-band distributions).
3. **Interactive Filtering** — **Slicers** are implemented across key dimensions (department, job role, attrition status) to enable dynamic, self-service drill-down without altering the underlying data model.
4. **Data Visualization** — Multiple chart objects translate aggregated metrics into visual KPIs, highlighting attrition concentration by department, compensation disparities, and satisfaction correlations.
5. **Executive Dashboard Layer** — A consolidated `Dashboard` sheet presents headline KPIs (Total Headcount, Total Leavers, Attrition Rate) alongside supporting visualizations, designed for at-a-glance consumption by non-technical stakeholders.

---

## Key Performance Indicators (KPIs)                         <img width="1100" height="691" alt="Screenshot 2026-07-01 122802" src="https://github.com/user-attachments/assets/2a64e372-78fa-4721-8281-da4ce3324c90" />


| Metric | Value |
|---|---|
| Total Headcount | **1,470** |
| Total Leavers | **237** |
| Attrition Rate | **16.12%** |

---

## Repository / Workbook Structure

```
HR_Attrition_Data_Analysis_Project.xlsx
│
├── Raw_Data          → Source-of-truth employee-level dataset (1,470 rows × 35 columns)
├── Calculations      → PivotTable-driven aggregation and derived metric layer
└── Dashboard         → Executive-facing visualization and KPI summary layer
```

---

## Business Impact & Strategic Value

This analysis provides HR and business leadership with a **critical decision-support tool** to:

- Prioritize retention interventions toward the departments and roles exhibiting the highest attrition concentration
- Evaluate whether **compensation misalignment** or **engagement deficits** are the primary attrition drivers, informing whether retention budget should target pay equity or culture initiatives
- Monitor attrition rate as an ongoing **workforce health KPI**, integrated into recurring HR operating reviews
- Reduce **unplanned turnover costs** by enabling earlier identification of at-risk employee segments

---

## Tools & Technologies

- **Microsoft Excel** — PivotTables, PivotCharts, Slicers, dashboard design
- **Data Analysis Techniques** — descriptive statistics, cross-tabulation, correlation-driven segmentation
- **Data Visualization** — KPI cards, comparative and distribution charts

---

## Future Enhancements

- Integrate **predictive modeling** (e.g., logistic regression or classification algorithms) to generate individual attrition-risk scores
- Automate data refresh via **Power Query** for continuous pipeline updates
- Extend the dashboard to **Power BI** for enhanced interactivity and enterprise-wide distribution
- Incorporate exit-interview sentiment data for qualitative root-cause analysis

---

## Author's Note

This project was developed as a demonstration of applied **HR analytics** and **business intelligence** capability — showcasing the ability to translate raw operational data into strategic, executive-level insight that directly supports workforce planning and organizational retention strategy.
