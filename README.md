🏥 Hospital Efficiency Analysis (Power BI + SQL)
📊 Project Overview

This project analyzes hospital patient data to understand patient admissions, hospital workload, department performance, and treatment patterns.

The analysis was performed using SQL for data exploration and Power BI for interactive dashboard visualization.

The goal of this project is to demonstrate data cleaning, data analysis, and data visualization skills in a real-world healthcare dataset.

🛠 Tools & Technologies

SQL – Data exploration and analysis

Power BI – Interactive dashboard creation

Power Query – Data cleaning and transformation

Data Visualization – Business insights generation

📁 Dataset Description

The dataset contains hospital patient records including:

Patient ID

Hospital Code

Department

Admission Type

Severity of Illness

Age Group

Bed Grade

Visitors with Patient

Admission Deposit

Length of Stay

City Code

This dataset helps analyze hospital efficiency and patient patterns.

🧹 Data Cleaning (Power Query)

The dataset was cleaned using Power Query by:

Removing null values

Fixing incorrect data types

Filtering inconsistent records

Removing duplicates

Standardizing column names

🗄 SQL Data Analysis

SQL queries were used to analyze the dataset before building the dashboard.

Examples of SQL analysis performed:

Total Patients
SELECT COUNT(patientid) AS total_patients
FROM train_data;
Patients by Department
SELECT department, COUNT(*) AS patient_count
FROM train_data
GROUP BY department
ORDER BY patient_count DESC;
Average Admission Deposit by Severity
SELECT severity_of_illness,
       AVG(admission_deposit) AS avg_deposit
FROM train_data
GROUP BY severity_of_illness;
Top 10 Cities with Most Patients
SELECT city_code_patient,
       COUNT(*) AS patient_count
FROM train_data
GROUP BY city_code_patient
ORDER BY patient_count DESC
LIMIT 10;

These queries helped identify patterns before creating visualizations.

📊 Power BI Dashboard

The interactive dashboard was built in Power BI and contains two pages.

1️⃣ Hospital Operations Overview

This page provides a high-level summary of hospital operations.

Key KPIs

Total Patients: 314K

Total Hospitals: 32

Average Admission Deposit: 4882

Average Visitors: 3.28

Visualizations

Admissions by Type

Patient Volume by Department

Bed Grade Distribution

Patient Distribution by City (Top 10)

Patient Distribution by Severity Level

2️⃣ Hospital Patient Insights (Deep Analysis)

This page provides deeper patient analysis.

Visualizations

Patient Distribution by Age Group

Patients by Hospital

Hospital Stay Duration

Visitors vs Admission Deposit

Average Admission Deposit by Severity

🔎 Key Insights

Trauma admissions represent the largest share of hospital cases.

Gynecology department handles the highest patient volume.

Moderate severity cases dominate hospital admissions.

Patients aged 31–50 represent the largest patient group.

Admission deposits increase slightly with illness severity.

Patient demand is concentrated in a few cities.

📷 Dashboard Preview
Overview Dashboard

Deep Analysis Dashboard

📂 Project Structure
Hospital-Patient-Analysis
│
├ dataset
│   hospital_data.csv
│
├ dashboard
│   hospital_dashboard.pbix
│
├ sql
│   hospital_queries.sql
│
├ images
│   overview_dashboard.png
│   deep_analysis_dashboard.png
│
└ README.md
📌 Skills Demonstrated

Data Cleaning

SQL Data Analysis

Power BI Dashboard Design

Data Visualization

Business Insight Generation

👨‍💻 Author

Mohammed Ibad
Aspiring Data Analyst

Skills:

Python

SQL

Excel

Power BI

Data Visualization
