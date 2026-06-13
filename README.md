🏥 Emergency Room Visits — Data Cleaning Project
Internship: DecodeLabs
Tools: Microsoft Excel

📋 Project Overview
This project demonstrates end-to-end data cleaning on a simulated Emergency Room (ER) visits dataset. The raw dataset contained multiple real-world data quality issues — including inconsistent formatting, invalid clinical values, missing entries, and duplicate records — that would compromise any downstream analysis or reporting if left unaddressed.
The goal was to transform a messy, unreliable dataset into a clean, analysis-ready file while documenting every decision made.

🗂️ 
Raw dataset: 1,021 rows × 11 columns
Clean dataset: 1,002 rows × 11 columns

🚨 Data Quality Issues Found
1. Inconsistent Categorical Values

2. Invalid Clinical Values

3. Missing Values
The raw dataset contained nulls across multiple columns

4. Duplicate

5. Column Naming & Formatting
Inconsistent casing and spacing in column headers standardised
Verbose column names shortened for clarity (e.g., Length Of Stay(hours) from LOS_Hrs)

🧹 Cleaning Steps Performed

Removed duplicate rows based on Visit ID
Standardised categorical fields — Gender, Severity, Insurance Type — using find-and-replace and consistent titling
Removed invalid age entries — negative values and physiologically implausible outliers (age > 120)
Handled missing values — retained rows with minimal missingness; rows with critical missing fields were flagged
Renamed columns for clarity and consistency
Validated diagnosis field — confirmed 8 valid diagnosis categories present with no anomalies

💡 Key Insights from Cleaning
Nearly 1 in 3 categorical entries in the raw file had formatting inconsistencies
30 missing wait times could significantly skew operational efficiency analysis if imputed incorrectly
Negative and extreme ages highlight the importance of data validation at the point of entry in clinical systems
The clean dataset reduced from 1,021 to 1,002 records — a 1.9% reduction from deduplication and invalid value removal
