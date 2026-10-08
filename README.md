# Hospital Readmission Analysis – Excel Data Analytics Project

## Project Overview

This project analyzes hospital encounter data to identify patterns and factors associated with 30-day patient readmissions.

The analysis was performed using Microsoft Excel with PivotTables, helper calculations, correlation analysis, and data visualizations.

## Business Problem

Hospitals need to understand factors associated with patient readmissions to support better patient care, discharge planning, follow-up processes, and resource allocation.

## Dataset

The dataset contains hospital encounter-level information including patient demographics, hospital utilization, medication-related information, diagnosis-related fields, and readmission status.

- Total Encounters Analyzed: **66,587**
- Overall Readmission Rate: **46.20%**
- Average Hospital Stay: **4.40 days**

## Tools Used

- Microsoft Excel
- PivotTables
- Excel Formulas
- Data Cleaning
- Correlation Analysis
- Data Visualization

## Key Analysis

### Age vs Readmission

Readmission rates were compared across different patient age groups. The 70–80 and 80–90 age groups showed relatively high readmission rates of approximately 48%.

### Medical Specialty vs Hospital Stay

Average hospital stay was analyzed across medical specialties.

The overall average hospital stay was approximately **4.40 days**. Pediatrics-Pulmonology showed an average stay of approximately **10.69 days**.

### Previous Emergency Visits vs Readmission

Previous emergency visits showed a weak positive correlation with readmission.

**Correlation: 0.17**

### Diabetes Medication vs Readmission

Encounters where diabetes medication was prescribed were analyzed.

- Encounters: **51,205**
- Readmission Rate: **47.96%**

### Medication Change vs Readmission

Readmission rates were compared between encounters with and without medication changes.

- Change = Yes: **48.62%**
- Change = No: **44.13%**
- Difference: **4.49 percentage points**

### Race and Gender vs Readmission

Overall readmission rates were:

- Female: **46.85%**
- Male: **45.44%**

### Weight vs Readmission

A major data-quality limitation was identified:

**96.80% of weight values were missing.**

Only approximately **3.20%** of weight records were available.

### Number of Medications vs Hospital Stay

Average hospital stay generally tended to increase with higher medication counts, although the relationship was not perfectly linear.

### Previous Outpatient Visits vs Readmission

- 0 visits: **43.78%**
- 1 visit: **57.76%**
- 2 visits: **59.94%**

The difference between 0 and 1 previous outpatient visit was approximately **13.98 percentage points**.

### Laboratory Procedures vs Readmission

The correlation between laboratory procedures and readmission was approximately:

**0.08**

This indicates a very weak positive relationship.

### Temporal Trend Analysis

Monthly and seasonal trend analysis could not be performed because admission and discharge date fields were not available in the dataset.

### Diagnostic Burden / Comorbidity

`number_diagnoses` was used as a proxy for diagnostic burden/comorbidity.

Comorbidity Score 7 showed an average hospital stay of approximately **6.14 days**.

Comorbidity Score 9 represented the largest analyzed group with **61 encounters**, an average hospital stay of approximately **5.18 days**, and a readmission rate of **44.26%**.

## Key Insights

- Overall readmission rate was approximately **46.20%**.
- Previous emergency and outpatient utilization showed noticeable positive patterns with readmission.
- Laboratory procedures showed only a very weak correlation with readmission.
- Medication changes were associated with a **4.49 percentage-point** difference in readmission rates.
- Medical specialty showed substantial variation in average hospital stay.
- Weight analysis was strongly limited by missing data.
- Diagnostic burden did not show a simple linear relationship with readmission or hospital stay.

## Data Limitations

- Admission and discharge dates were not available.
- Approximately 96.80% of weight values were missing.
- Some categories contained very small sample sizes.
- The analysis is primarily descriptive.
- Correlation does not imply causation.
- `number_diagnoses` is used as a proxy for diagnostic burden and is not a clinically validated comorbidity index.

## Business Recommendations

- Identify patients with higher previous healthcare utilization for closer follow-up.
- Investigate specialties with longer average hospital stays for resource planning.
- Improve completeness of patient weight information.
- Collect admission and discharge dates for future temporal analysis.
- Use statistical testing and predictive modelling in future analysis.

## Project Structure

The Excel workbook contains:

- Cover
- Raw_Data
- Data_Dictionary
- Data_Cleaning
- Helper_Data
- Analysis
- Pivot_Analysis
- Dashboard
- Insights

## Conclusion

This project demonstrates the use of Microsoft Excel for healthcare data analysis, including data preparation, PivotTable analysis, correlation analysis, visualization, interpretation, and business recommendations.

The findings provide descriptive insights into factors associated with hospital readmission while highlighting important data-quality and analytical limitations.
