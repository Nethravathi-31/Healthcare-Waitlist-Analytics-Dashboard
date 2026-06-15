🏥 Inpatient & Outpatient Healthcare Dashboard
📌 Project Overview

This project is an interactive Power BI Dashboard developed to analyze Inpatient, Outpatient, and Day Case hospital records over time.

The dashboard helps healthcare administrators and analysts monitor:

Patient admissions
Outpatient visits
Day case trends
Specialty-wise performance
Age group analysis
Time-band distribution
Monthly and yearly trends
🎯 Objectives
Analyze hospital cases across different case types.
Compare Inpatient, Outpatient, and Day Case volumes.
Identify high-performing specialties.
Understand patient distribution across age groups.
Track trends over time for better decision-making.
📊 Dashboard Pages
1. Summary Dashboard

The Summary page provides a high-level overview of hospital activities.

Key Features

✅ KPI Cards

Latest Month Wait List
Previous Year Latest Month Wait List

✅ Filters / Slicers

Archive Date
Case Type
Specialty Name

✅ Visualizations

Case Type Distribution (Donut Chart)
Average/Median Wait List by Age Profile and Time Bands
Specialty-wise Wait List Distribution (Pie Chart)
Trend Analysis of:
Inpatient
Day Case
Outpatient
2. Detail View Dashboard

The Detail View provides a detailed breakdown of hospital records.

Filters Available
Archive Date
Case Type
Specialty Name
Age Profile
Time Bands
Matrix Table

The matrix visual allows users to drill down through:

Year
 └── Quarter
      └── Month
            └── Day
                  └── Specialty
                        └── Age Profile
                              └── Time Band

Measures displayed:

Day Case Count
Inpatient Count
Outpatient Count
Total Cases
📈 Key Insights
Case Type Analysis
Outpatient cases contribute the highest proportion of total hospital records.
Inpatient and Day Case records form a smaller percentage compared to Outpatient visits.
Specialty Analysis
The dashboard identifies specialties with:
Highest patient volume
Longest waiting lists
Age-specific trends
Age Group Analysis

Patients are categorized into:

0–15 Years
16–64 Years
65+ Years

This helps understand which age groups require more healthcare resources.

Time Band Analysis

Patient wait lists are segmented into:

0–3 Months
3–6 Months
6–9 Months
9–12 Months
12–15 Months
15–18 Months
18+ Months

This helps track waiting periods and improve hospital efficiency.

🛠 Tools & Technologies
Tool	Purpose
Power BI	Data Visualization
Power Query	Data Transformation
DAX	Measures and Calculations
Excel / CSV	Data Source
Data Modeling	Relationships & Schema
📂 Data Model

The dashboard uses:

Fact Table
Hospital Cases
Wait List Records
Dimension Tables
Date Table
Specialty Table
Case Type Table
Age Profile Table
Time Band Table
📌 DAX Measures Used

Some important DAX measures include:

Total Cases =
SUM(FactHospital[Total])

Inpatient Cases =
CALCULATE(
    SUM(FactHospital[Total]),
    FactHospital[Case_Type] = "Inpatient"
)

Outpatient Cases =
CALCULATE(
    SUM(FactHospital[Total]),
    FactHospital[Case_Type] = "Outpatient"
)

Day Case =
CALCULATE(
    SUM(FactHospital[Total]),
    FactHospital[Case_Type] = "Day Case"
)
🚀 Business Impact

This dashboard helps hospitals to:

Monitor patient inflow efficiently.
Identify specialties with high demand.
Reduce waiting times.
Allocate resources effectively.
Improve patient care through data-driven decisions.
📷 Dashboard Preview
Summary Dashboard
KPI Cards
Case Type Distribution
Age Profile Analysis
Specialty Analysis
Trend Analysis
Detail Dashboard
Interactive Filters
Drill-down Matrix
Specialty-wise and Age-wise Breakdown
