# Amalitech-HR-Analytics-Dashboard

### Dashboard Link: [Power BI Report](https://app.powerbi.com/groups/me/reports/your-dashboard-link-here/ReportSection)

## Problem Statement

This HR Analytics Dashboard was created to provide AmaliTech with a comprehensive overview of workforce trends, performance metrics, and employee demographics. It enables HR leadership to identify strengths, gaps, and risk areas across departments and regions—empowering evidence-based decision-making.

By visualizing key indicators such as gender distribution, contract types, recruitment channels, awards, training, service years, and KPI achievements, AmaliTech can better align HR initiatives with strategic goals. The dashboard also surfaces early warnings such as at-risk talent pools and underperforming locations, allowing for proactive interventions.

## Key Metrics

- **Total Employees:** 23,000  
- **KPI Met Rate:** 35.9%  
- **Average Rating:** 3.31  
- **Average Service Years:** 5.81  
- **Total Award Winners:** 535  

## Data Preparation (Power Query Steps)

Before building the visualizations, the raw dataset underwent transformation in Power Query with the following steps:

1. **Source**: Connected to the raw data file (likely Excel or CSV).
2. **Navigation**: Navigated to the appropriate sheet/table.
3. **Promoted Headers**: Converted the first row of data into column headers.
4. **Changed Type**: Automatically detected and assigned appropriate data types (e.g., text, number, date).
5. **Replaced Value**: Handled initial cleanup (e.g., fixing inconsistent gender labels or education levels).
6. **Replaced Value1**: Further replacements, likely for contract types or department naming consistency.
7. **Replaced Value2**: Final cleanup pass for nulls, typos, or category standardization.

## Steps Followed

- **Step 1**: Loaded HR dataset (CSV format) into Power BI Desktop.
- **Step 2**: Used Power Query Editor to inspect column distribution, data quality, and column profiles across the full dataset.
- **Step 3**: Cleaned null and invalid values across fields such as `AtRisk`, `Flight Distance`, and `Education`.
- **Step 4**: Applied business logic to calculate custom fields:
  - **Age Group Classification** (e.g., 20–30, 31–40).
  - **KPI Status**, **High Performer Category**, and **At-Risk Flags**.
- **Step 5**: Designed visuals for:
  - **Contract Types** (Full-Time vs Part-Time)
  - **Recruitment Channels** (Company website vs Social networks)
  - **Gender Distribution**
  - **Awards and Training by Department**
  - **Age Distribution Histogram**
  - **KPI Met Rates by Department**
- **Step 6**: Added slicers for key dimensions: `Location`, `Education`, `Department`, `Gender`, `Contract Type`, and `Recruitment Channel`.
- **Step 7**: Created DAX measures:
  - `% of KPIs Met`
  - `Total Employees`
  - `Total Awards`
  - `Total At-Risk Count`
  - `Average Service Years`
  - `Training Volume by Department`
- **Step 8**: Included interactive tables for:
  - **Employee Watchlist (At-Risk)**
  - **Employee Count by Department and Location**
  - **High vs Low Performing Departments**
- **Step 9**: Published report to Power BI Service and applied appropriate workspace access controls.

## Insights

### 1. Workforce Composition

- **64.03%** of employees are **Full-Time**, **35.97%** are **Part-Time**.
- Recruitment is primarily through the **Company’s Website (57%)**, followed by **Social Networking (42%)**.
- Gender split: **70.65% Female**, **29.3% Male**.

### 2. KPI & Performance Trends

- **Overall KPI Met Rate**: 35.9%
- Top KPI Departments: `Operations (44.4%)`, `Research & Development (44.1%)`, `Analytics (40.4%)`.
- Bottom KPI Departments: `Sales & Marketing (27.6%)`, `Legal (34.2%)`.

### 3. Awards & Training

- `Sales & Marketing` won the most awards (153).
- Most training investments also go to `Sales & Marketing` (9,277 sessions).

### 4. Risk Watchlist

- **Total at-risk employees:** 1,059
- Top at-risk department: `Sales & Marketing (875)`

### 5. Employee Tenure

- Longest serving departments: `Operations (6.41 years)` and `Procurement (6.24 years)`.
- Shortest average tenure: `Legal (4.6 years)` and `R&D (4.75 years)`.

### 6. High vs Low Performers

- **Top Performing Departments**: `Technology`, `Analytics`, `R&D`.
- **Least Performing Departments**: `Procurement`, `Finance`, `HR`.
- **Top Locations**: `Ashaiman`, `Sunyani`, `Obuasi`, `Cape Coast`.
- **Least Performing Locations**: `Elmina`, `Nkawkaw`, `Berekum`.

## Snapshots


![WhatsApp Image 2025-05-22 at 07 48 10_92cf6977](https://github.com/user-attachments/assets/1536b355-a79b-4f56-b206-c893298bbf0a)![WhatsApp Image 2025-05-22 at 07 48 10_a0dd1a03](https://github.com/user-attachments/assets/46998fc9-1de9-40a9-86f7-33da2811bd9a)



