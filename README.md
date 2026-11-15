# Smoking and Health Analysis Dashboard

## Project Overview
An interactive healthcare analytics dashboard developed in **Microsoft Power BI** for the Sapphire IQ project scenario. It explores patient smoking patterns, recorded health conditions, organ categories, blood pressure risk groupings, cholesterol, demographics, and estimated smoking exposure.

This project is intended for educational and exploratory analysis. It does **not** establish medical diagnoses or prove that smoking causes any specific health condition.

## Objectives
1. Summarise patient records using key performance indicators (KPIs).
2. Create DAX calculated columns for age groups and blood-pressure risk categories.
3. Explore smoking patterns and health indicators.
4. Compare patient demographics and recorded health-condition patterns across estimated smoking-exposure levels.

## Dashboard Contents

### KPI cards
- Total Patients
- Total Current Smokers
- Patients with Recorded Organ Category
- Patients with Recorded Health Conditions

### Slicers
- Region
- Gender
- Age Group

### Six charts
1. Average Cigarettes Consumed Per Day by Smoking Status
2. Smoking Status Distribution
3. Organ-wise Health Condition Distribution
4. Average Cholesterol Levels by BP Risk Category
5. Number of Current Smokers Across Age Groups
6. Distribution of Health Conditions by Smoking Exposure Level

### Patient summary table
A table visual is included to display patient-level summary fields selected for the report.

## Data Fields Used
The dataset includes fields such as Age, BMI, Cigarettes_Per_Day, Diagnosed_Organ, Diagnosis_Date, Diastolic_BP_mmHg, Gender, Health_Condition, Patient_ID, Region, Resting_Heart_Rate_bpm, Smoking_Status, Systolic_BP_mmHg, Total_Cholesterol_mg_dL, and Years_Smoking.

## DAX Calculations

### Age Group
Patients are grouped into 18–29, 30–44, 45–59, and 60+ age bands.

### BP Risk Category
The report uses systolic and diastolic blood-pressure readings to group records into Lower Range, Elevated, and High. The thresholds used in this project are analytical assumptions because the project brief does not specify cut-offs. They are not medical advice or diagnostic criteria.

### Estimated Smoking Exposure
Estimated exposure is calculated as:

`(Cigarettes_Per_Day / 20) × Years_Smoking`

This is an estimated pack-year style measure, assuming 20 cigarettes per pack.

### Smoking Exposure Level
The project groups estimated exposure into Low (<5), Moderate (5 to <15), and High (15 or more). These are project-defined bands for exploratory comparison, not clinical thresholds.

## Tools
- Microsoft Power BI Desktop
- DAX
- GitHub

## Repository Files
Add the following project files to this repository:
- `Smoking_Health_Analysis.pbix` — editable Power BI report
- `Smoking_Health_Analysis_Dashboard.pdf` — exported dashboard
- `Dashboard_Screenshot.png` — dashboard preview
- `Project_Documentation.pdf` — project report
- `README.md` — project overview
- `.gitignore` — files excluded from version control
- `LICENSE` — license for the project documentation and original project materials

## Important Notes
- KPI values depend on the loaded dataset and active report filters/slicers.
- Check that all slicers and filters are cleared before recording final overall KPI values.
- Do not publish patient-identifiable, confidential, or restricted data. Only upload datasets you are authorised to share.
- The dataset itself may have separate ownership or licensing terms; this repository license does not grant rights to redistribute third-party data.

## How to View
1. Download `Smoking_Health_Analysis.pbix`.
2. Open it using Microsoft Power BI Desktop.
3. Use the Region, Gender, and Age Group slicers to explore the report.
