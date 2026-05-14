# 🏥 Hospital-Patient-Records
This project is a hospital patient records data analysis using Microsoft Excel with the aim of identifying patient encounter patterns, healthcare cost trends, and clinical insights that can assist in data-driven decision making.

## ✨ Project Goals
Think of this as a Healthcare Analytics task. The Goals Are to:
1. Measure total patient encounters and total healthcare costs across all records
2. Know the average cost per encounter and average payer coverage rate
3. Identify the most common encounter types based on frequency
4. Determine the Top 10 most frequent diagnoses (Reason Descriptions)
5. Analyze encounter trends over time to identify seasonal or periodic patterns
6. Evaluate cost and encounter distributions based on:
     - Encounter Class (ambulatory, emergency, inpatient, wellness, urgentcare)
     - Payer / Insurance Provider
7. Generate actionable healthcare insights that can be used to optimize hospital resource allocation and cost management strategies

## ❓ Business Questions
### 🔢 Encounter & Cost Performance
- What is the total number of patient encounters during the selected period?
- How much total claim cost was generated across all encounters?

### 🏨 Encounter Type Performance
- Which encounter class generates the highest total claim cost?
- What are the Top 10 most frequent diagnoses?
- Do inpatient encounters contribute significantly more to total costs compared to ambulatory visits?

### 📈 Trend Analysis
- How does encounter volume change month by month?
- Are there any seasonal patterns or peak admission periods?
- Which months show the highest and lowest encounter volumes?

## 📦 Dataset Overview
- **Source**: [Hospital Patient Records](https://mavenanalytics.io/data-playground/hospital-patient-records)
- **Sheets**: 5 data tables + data dictionary + pivot tables + dashboard

| Sheet | Rows | Columns | Description |
|---|---|---|---|
| encounters | 27,891 | 16 | Patient visit/encounter records |
| patients | 974 | 20 | Patient demographic data |
| procedures | 47,701 | 10 | Medical procedures performed |
| payers | 10 | 7 | Insurance payer information |
| organizations | 1 | 8 | Hospital/organization details |

**Key Feature Groups**
- **Encounter Information**: `Id`, `START`, `STOP`, `ENCOUNTERCLASS`, `CODE`, `DESCRIPTION`, `BASE_ENCOUNTER_COST`, `TOTAL_CLAIM_COST`, `PAYER_COVERAGE`, `REASONCODE`, `REASONDESCRIPTION`
- **Patient Information**: `Id`, `BIRTHDATE`, `DEATHDATE`, `GENDER`, `RACE`, `ETHNICITY`, `MARITAL`, `CITY`, `STATE`
- **Procedure Information**: `ID_PROCEDURE`, `PROCEDURE_DESCRIPTION`, `START`, `STOP`
- **Payer / Insurance**: `Id`, `Name`, `Address`, `Phone`

## 🧹 Data Cleaning and Preparation
Cleaning was performed in Microsoft Excel:
- Ensured numeric columns (cost, coverage) were correctly formatted
- Cleaned and validated categorical data (encounter class, gender, race)
- Removed or flagged duplicate encounter records
- Prepared relational joins across patients, encounters, procedures, and payers for aggregation and trend analysis

## 📊 Dashboard Microsoft Excel
A one-page interactive dashboard was created to visualize hospital patient data

### **Dashboard Highlights**
  - KPI Cards
      - Total Encounters
      - Total Patient
      - Total Procedures
  - Segments Chart
      - Encounters by Class (ambulatory, emergency, inpatient, wellness, urgentcare)
      - Top 10 Most Frequent Diagnoses
      - Monthly Encounter Trend
      - Cost Breakdown
  - Slicer for quick exploration
      - `ENCOUNTERCLASS`, `START`, `MONTH`

Dashboard Preview:

> `![Dashboard Preview](Hospital-Patient-Records-Dashboard.png)`

## 🛠️ Tools Used
- Microsoft Excel:
    - Data Cleaning & Preparation
    - Pivot Table for creating graphs and aggregations
    - Dashboarding with slicers and KPI cards

## 🙌 Thanks for Reading!
