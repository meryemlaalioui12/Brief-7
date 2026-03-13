HR Workforce Analytics Dashboard

Built with Power BI | Simplon Academy


Overview
The HR Workforce Analytics Dashboard is a multi-page Power BI report designed to provide HR teams and business leaders with a comprehensive view of workforce composition, headcount trends, retention, and turnover. It enables data-driven decision-making through interactive filters and drill-through capabilities.

Dashboard Pages
Home
A high-level summary page with bookmarked views for quick navigation.
Page 1 – Workforce Overview
The main analytics page containing all key visuals described below.

Key Metrics (KPI Cards)
MetricDescriptionAll EmployeesTotal headcount across the organizationHeadcountCurrent active headcountStarting HeadcountHeadcount at the beginning of the selected periodEnding HeadcountHeadcount at the end of the selected period

Visualizations
VisualDescriptionHeadcount by Job Level & DepartmentStacked bar chart breaking down employees across job levels (CEO, Director, Manager, Team Lead, Individual Contributor) by departmentHeadcount by Location & DepartmentStacked bar chart comparing Remote vs. On-site employees per departmentHeadcount by Location CityMap visual showing geographic distribution of employees across the United StatesHeadcount by Marital StatusDonut chart showing split between Married (50%) and Single (50%) employees

Filters / Slicers
The report includes the following interactive filters on the left panel:

Year – Filter data by year (default: 2017)
Race – Filter by employee race
Gender – Filter by gender
Department – Filter by department
Education – Filter by education level
Job Level – Filter by job level
Birth Date – Filter by date of birth range
Marital Status – Filter by marital status
Location City – Filter by city


Data Model
Dimension Tables

Job Level Dim – Job Key, job_level
Location Dim – location, Location Key, location_city
Manager Dim – Manager-related attributes
Marital Dim – Marital Key, marital_status
Termination Dim – Termination-related attributes

Measures Table (MesuresTable)

All Employees
Employees Left
Ending Headcount
Headcount
Retention
Starting Employees
Starting Headcount
Turnover
Value


Bookmarks
Three bookmarks are configured for quick navigation between report states:

Headcount – Jumps to headcount overview
Retention – Jumps to retention view
Turnover – Jumps to turnover view


Drill-Through
The report supports drill-through with cross-report enabled. Drill-through fields can be configured to filter visuals based on selected data points.

Notes

The map visual (Headcount by location_city) uses a visual type that is being retired in Power BI. Contact your admin to upgrade to the latest map visual.
All KPI cards reference measures from MesuresTable to ensure consistency across filters.
The report file is named Brief-7 and contains 2 pages.


Requirements

Power BI Desktop (latest version recommended)
Data source connection to the HR dataset (tables: Job Level Dim, Location Dim, Manager Dim, Marital Dim, Termination Dim, MesuresTable)
