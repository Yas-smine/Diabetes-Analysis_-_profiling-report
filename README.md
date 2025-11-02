
# 🩺 Diabetes Dataset Profiling & Comparative Analysis

This repository documents a complete data exploration and profiling workflow for the Pima Indians Diabetes Dataset. The goal is to uncover patterns, correlations, and data quality issues that may influence diabetes diagnosis.

## 📁 Repository Contents
- `Diabetes_Dataset_Analysis.ipynb`: Main notebook for data cleaning and profiling
- `Diabetes_Dataset_Analysis_2.ipynb`: Alternate profiling run for comparison
- `comparing_reports.ipynb`: Comparative analysis of profiling outputs
- *(Optional)* `profiling_report.html`: Exported interactive report

## 📊 Dataset Description
The dataset includes medical and demographic indicators relevant to diabetes diagnosis:
- `Pregnancies`: Number of times the patient was pregnant
- `Glucose`: Plasma glucose concentration
- `BloodPressure`: Diastolic blood pressure (mm Hg)
- `SkinThickness`: Triceps skinfold thickness (mm)
- `Insulin`: 2-Hour serum insulin (mu U/ml)
- `BMI`: Body Mass Index (kg/m²)
- `DiabetesPedigreeFunction`: Genetic influence score
- `Age`: Patient age (years)
- `Outcome`: Diabetes diagnosis (0 = No, 1 = Yes)

## 🧪 Step 1: Data Exploration with Pandas
- Loaded dataset and displayed structure (column names, types, memory usage)
- Identified zero values in key columns (`Glucose`, `BloodPressure`, `BMI`, `Insulin`)
- Used `.describe()` to analyze summary statistics and detect unrealistic values

## 📈 Step 2: Profiling with ydata-profiling
- Generated interactive profiling reports for both cleaned and raw datasets
- Explored column types, distributions, missing values, and outliers
- Analyzed correlation matrices to identify relationships (e.g., `Glucose` vs `Outcome`)
- Compared profiling outputs across notebooks to validate consistency

## 🧵 Step 3: Summary of Findings
- Higher glucose and BMI levels are associated with diabetes diagnosis
- `Pregnancies` and `Age` show moderate influence on `Outcome`
- Zero values in medical fields suggest missing data requiring imputation
- Profiling reports flagged skewed distributions and potential outliers

## ✅ Suggestions & Next Steps
- Replace or impute zero values in critical columns
- Consider scaling or transforming skewed features
- Explore predictive modeling (e.g., logistic regression, decision trees)
- Visualize key relationships using plots or dashboards (e.g., Tableau)

## 🛠️ Tools Used
- Python, Pandas, NumPy
- ydata-profiling (`pandas-profiling`)
- Jupyter Notebook

---

📌 _This analysis supports future modeling and reporting tasks in healthcare analytics. All notebooks are structured for reproducibility and comparison._
