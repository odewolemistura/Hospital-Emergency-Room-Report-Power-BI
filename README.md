# 🏥 Hospital Emergency Room Report – Power BI

## Table of Contents

- [Project Overview](#project-overview)
- [Data Description](#data-description)
- [Tools Used](#tools-used)
- [Data Cleaning & Preparation](#data-cleaning--preparation)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Data Analysis & Dashboard Design](#data-analysis--dashboard-design)
  - [Monthly Overview](#monthly-overview)
  - [Total Overview](#total-overview)
- [Key Findings](#key-findings)
- [Recommendations](#recommendations)



## Project Overview
This project explores a hospital emergency room dataset to gain insights into patient trends, satisfaction levels, wait times, and referral patterns. Using Power BI, a dynamic dashboard was created to support both **monthly** and **total period analyses**, enabling hospital administrators to optimize operations and resource allocation.

##  Data Description
The dataset contains **9,216** unique patient records spanning a period of **19 months**, from **April 2023 to September 2024**. It includes the following columns:

- `Patient ID`
- `Patient Admission Date`
- `Patient First Initial`
- `Patient Last Name`
- `Patient Gender`
- `Patient Age`
- `Patient Race`
- `Department Referral`
- `Patient Admission Flag`
- `Patient Satisfaction Score`
- `Patient Wait Time`
- `Patients CM`

##  Tools Used
- **Power BI** for visualization and analysis  
- **Power Query** for data cleaning  
- **DAX** for calculated columns and measures  
- **Date Table** (custom created) for time intelligence
  
##  Data Cleaning & Preparation
- Merged relevant fields such as first name initial and last name for full name.
- Created a **custom Date table** for proper time-based slicing.
- Cleaned inconsistent formats and null values using **Power Query**.
- Created **DAX measures** for KPIs like:
  - Number of patients  
  - Average wait time  
  - Average satisfaction score  
  - Total patients referred  
  - % of patients seen within 30 minutes  

##  Exploratory Data Analysis (EDA)
Conducted EDA to identify:
- Admission trends by time (monthly, hourly, daily)
- Patient demographics by gender, age group, and race
- Referral distribution across departments
- Wait time distribution
- Admission vs. non-admission rate

## Data Analysis & Dashboard Design

### Monthly Overview
**Slicer:** `Month`

- Number of patients per month  
- Admission status breakdown  
- Gender distribution  
- % seen within 30 minutes  
- Age group analysis  
- Day/hour heatmap  
- Referral department stats  
- Racial composition  

### Total Overview
**Slicer:** `Start Date - End Date (Calendar Range)`

- Replicates the above analyses for any custom time range

## Key Findings
- **High patient volume** observed on **Mondays** and during **late night to early morning** hours.
- **Moderate satisfaction scores**, with potential to improve.
- Most common department referrals were **General Practice** and **Orthopedics**.
- **Diverse demographic composition** in terms of race and age group.
- Nearly **equal distribution** between **admitted** and **non-admitted** patients.

## Recommendations
- **Increase staff coverage** during peak times (especially Mondays and late nights).
- **Targeted improvements** in departments with lower satisfaction scores.
- **Streamline referral processes** for General Practice and Orthopedics.
- Consider strategies to reduce wait time for improved patient experience.





