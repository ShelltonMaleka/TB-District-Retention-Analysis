# TB Patient Retention Analysis in South Africa
## Project Overview
Tuberculosis (TB) treatment requires patients to remain in continuous care for treatment to be successful. Patients who are lost to follow-up may experience interrupted treatment, making retention an important part of TB control.
This project uses district-level South African health data to investigate the factors associated with the inability to retain drug-susceptible TB patients in continuous care.
## Research Question
Which variables are most strongly associated with a district's inability to retain drug-susceptible Tuberculosis (TB) patients in continuous care in 2024?
The main outcome variable is: TB DS client lost to follow-up rate 
A higher lost-to-follow-up rate represents poorer patient retention.
## Data Source 
The analysis uses data extracted from the District Health Barometer (DHB) 2024/25, published by Health Systems Trust.

**The final dataset contains:**
- 52 South African health districts
- 11 variables
- 8 numerical explanatory variables
- 1 target variable
- Province and district identifiers

**The explanatory variables considered were:**
- TB DS death rate
- TB/HIV co-infected clients on ART rate
- Percentage of the target tested for TB
- Professional nurses per 100 000 population
- District Health Services expenditure per capita for the uninsured population
- PHC expenditure per PHC headcount
- Expenditure per patient day equivalent at district hospitals
- Average medical scheme coverage
## Project Workflow
The analysis followed the workflow below:
```text
District Health Barometer Data
↓
Data Extraction
↓
WHO-Based Data Quality Audit
↓
Data Cleaning and Preprocessing
↓
Exploratory Data Analysis
↓
Correlation Analysis
↓
Multiple Linear Regression
↓
Model Evaluation
↓
Interpretation of TB Patient Retention Factors
```
---
## Data Quality Audit
Before performing the analysis, the dataset was assessed using principles from the World Health Organization Data Quality Review framework.
The audit included checks for:
- Missing values
- Duplicate observations
- Data types
- Consistency
- Numerical ranges
- Potentially unusual values

There were no duplicate records and no missing values in the numerical variables used for modelling.

The ```geo_prov``` variable contained 43 blank entries because of the structure of the original DHB table. Province names were listed once followed by the districts belonging to that province. These were therefore treated as structural blanks and forward-filled.
Unusually large numerical values were investigated rather than automatically removed because unusual observations are not necessarily data errors.
**All 52 districts were retained for the final analysis.**
## Exploratory Data Analysis

EDA was performed using:
- Descriptive statistics
- Histograms
- Boxplots
- Scatterplots
- Correlation analysis
- Correlation heatmaps

The strongest individual correlations with TB lost-to-follow-up rate were:

| Variables| Pearson Correlation |
|----------|---------------------|
|% of target tested for TB| -0.521|
|Medical scheme coverage	|0.463|
|TB DS death rate	|-0.434|
|PHC expenditure per PHC headcount	|-0.228|
|Professional nurses per 100 000	|-0.189|
|Expenditure per patient day equivalent	|-0.187|
|TB/HIV co-infected clients on ART	|-0.046|
|District Health Services expenditure per capita	|0.028|





