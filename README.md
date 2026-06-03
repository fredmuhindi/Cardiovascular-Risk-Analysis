Cardiovascular Risk Analysis
Overview
This project analyzes demographic, biometric, and lifestyle data to identify patterns and risk factors associated with cardiovascular disease (CVD). Using a dataset of 1,529 individuals across 22 variables, the analysis explores how age, body composition, blood pressure, cholesterol, and lifestyle habits relate to cardiovascular health outcomes.

Dataset
The dataset captures a broad range of health indicators, including:

Demographics: Sex, Age
Anthropometrics: Weight, Height, BMI, Abdominal Circumference, Waist-to-Height Ratio
Blood Pressure: Systolic BP, Blood Pressure Category
Lipid Profile: Total Cholesterol, Estimated LDL
Metabolic: Fasting Blood Sugar
Lifestyle: Physical Activity Level, Family History of CVD
Derived Risk Metrics: CVD Risk Score, CVD Risk Level


Data composition: 14 numerical variables and 8 categorical variables. Missing values were present in several numerical fields and were imputed using median (numerical) and most-frequent (categorical) strategies.


Analysis Workflow
1. Data Cleaning

Inspected dataset structure and data types
Identified and imputed missing values using sklearn.impute.SimpleImputer
Verified no duplicate records

2. Exploratory Data Analysis (EDA)
Key visualizations include:

Age Distribution — bar chart showing the spread of participants by age
BMI Distribution — histogram with KDE to reveal body weight patterns
Systolic BP by Blood Pressure Category — boxplots comparing BP levels across categories
Age by CVD Risk Level — boxplots showing how risk varies with age
Age vs. BMI — scatter plot exploring the relationship between age and body mass
Age vs. Systolic BP by CVD Risk Level — scatter plot with risk-level hue
Age vs. Total Cholesterol — scatter plot tracking cholesterol trends across age groups


Key Findings

Age is a notable factor, with higher CVD risk levels concentrated in older age groups
BMI and systolic blood pressure show variation across CVD risk categories, suggesting their relevance as risk indicators
Cholesterol levels trend with age, highlighting the need for age-adjusted screening
Blood pressure categorization aligns well with measured systolic BP values, confirming data consistency


Tools & Libraries
LibraryPurposepandasData manipulationnumpyNumerical operationsmatplotlibBase plottingseabornStatistical visualizationssklearnMissing value imputation

How to Run

Clone this repository
Place the Cardiovascular Dataset.csv file in your working directory
Update the file path in the data import cell:

python   df = pd.read_csv("Cardiovascular Dataset.csv")

Run all cells in Cardiovascular_Risk_Analysis_.ipynb


Project Structure
├── Cardiovascular_Risk_Analysis_.ipynb   # Main analysis notebook
├── Cardiovascular Dataset.csv            # Source dataset (not included)
└── README.md                             # Project documentation

Author
Fredrick Waweru
