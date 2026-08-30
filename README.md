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
The final dataset contains:
- 52 South African health districts
- 11 variables
- 8 numerical explanatory variables
- 1 target variable
- Province and district identifiers
The explanatory variables considered were:
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
