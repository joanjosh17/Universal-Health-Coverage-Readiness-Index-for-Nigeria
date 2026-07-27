## Universal Health Coverage Readiness Index for Nigeria

### 📌 Overview

Universal Health Coverage (UHC) is a global health priority under Sustainable Development Goal (SDG) 3.8, ensuring that everyone has access to quality healthcare services without suffering financial hardship.

This project develops a Universal Health Coverage Readiness Index (UHCRI) for Nigeria using synthetic healthcare, demographic, infrastructure, and financing indicators. Through advanced data analytics and machine learning, the project evaluates healthcare readiness across Nigerian states, identifies disparities, predicts readiness categories, and provides insights that can support evidence-based health policy and strategic planning.

Note: This project uses a realistic synthetic dataset created solely for educational, research, and portfolio purposes.

Objectives

The project aims to:

Assess Universal Health Coverage readiness across Nigerian states.
Analyze healthcare infrastructure and workforce distribution.
Measure healthcare accessibility and financial protection.
Predict UHC readiness using machine learning.
Identify the most influential healthcare indicators.
Support evidence-based public health decision-making.
Demonstrate an end-to-end public health data science workflow.
Dataset

The synthetic dataset contains approximately 5,000 observations representing healthcare indicators across Nigeria.

Features
Feature	Description
Record_ID	Unique record identifier
State	Nigerian State
Area_Type	Urban or Rural
Population	Estimated population
Health_Facilities	Number of health facilities
Doctors_per_1000	Doctors per 1,000 population
Nurses_per_1000	Nurses per 1,000 population
Insurance_Coverage_pct	Health insurance coverage (%)
Immunization_Coverage_pct	Childhood immunization coverage (%)
Skilled_Birth_Attendance_pct	Skilled birth attendance (%)
Out_of_Pocket_Expenditure_pct	Household out-of-pocket expenditure (%)
Improved_Water_Access_pct	Access to improved water (%)
Electricity_Availability_pct	Health facility electricity availability (%)
Avg_Travel_Time_to_Facility_min	Average travel time to healthcare
UHC_Readiness_Index	Continuous readiness score (0–100)
Readiness_Category	Low, Moderate, High
Project Workflow
Synthetic Dataset
        │
        ▼
Data Cleaning
        │
        ▼
Exploratory Data Analysis
        │
        ▼
Feature Engineering
        │
        ▼
Machine Learning
        │
        ▼
Hyperparameter Tuning
        │
        ▼
Model Evaluation
        │
        ▼
Explainable AI (SHAP)
        │
        ▼
Prediction System
Exploratory Data Analysis

The project includes comprehensive EDA, including:

Missing value analysis
Duplicate detection
Descriptive statistics
Distribution analysis
Correlation analysis
Boxplots
Histograms
Pairplots
Urban vs Rural comparisons
State-level healthcare summaries
Feature Engineering

Several domain-inspired healthcare indicators were created:

Facilities per 100,000 population
Doctor availability score
Nurse availability score
Healthcare workforce density
Service coverage index
Infrastructure index
Financial protection index
Accessibility index
Accessibility risk classification
Insurance level categorization
Machine Learning Models
Classification Models
Logistic Regression
Decision Tree
Random Forest
Gradient Boosting
Extra Trees
XGBoost (Hyperparameter Tuned)

Classification target:

Readiness_Category
Regression Models
Linear Regression
Random Forest Regressor
Gradient Boosting Regressor
Extra Trees Regressor

Regression target:

UHC_Readiness_Index
Hyperparameter Tuning

The project uses

RandomizedSearchCV
Stratified K-Fold Cross Validation
Parameter optimization
Cross-validation performance evaluation
Explainable AI

The project incorporates explainable machine learning using SHAP to identify the healthcare indicators contributing most to readiness predictions.

Outputs include:

SHAP Summary Plot
SHAP Bar Plot
Global Feature Importance
Model Interpretation
Visualizations

The project generates numerous visualizations, including:

Correlation Heatmap
Distribution Plots
State Comparison Charts
Urban vs Rural Analysis
Feature Importance
SHAP Summary
SHAP Bar Plot
Confusion Matrix
ROC Curve
Precision–Recall Curve
Actual vs Predicted Plot
Residual Plot
Cross Validation Performance
UHC Readiness Distribution
Project Structure
Universal-Health-Coverage-Readiness-Index-for-Nigeria/

│
├── data/
│   └── Universal_Health_Coverage_Readiness_Index_Nigeria_Synthetic_Dataset.csv
│
├── models/
│   ├── final_xgboost_classifier.pkl
│   ├── best_regression_model.pkl
│   ├── preprocessor.pkl
│   └── label_encoder.pkl
│
├── outputs/
│   ├── figures/
│   └── reports/
│
├── src/
│   ├── data_preprocessing.py
│   ├── feature_engineering.py
│   ├── train_classification.py
│   ├── train_regression.py
│   ├── hyperparameter_tuning.py
│   ├── explainability.py
│   └── prediction.py
│
├── app.py
├── requirements.txt
├── README.md
└── LICENSE
Installation

Clone the repository

git clone https://github.com/yourusername/Universal-Health-Coverage-Readiness-Index-for-Nigeria.git

Move into the project directory

cd Universal-Health-Coverage-Readiness-Index-for-Nigeria

Install dependencies

pip install -r requirements.txt
Running the Project

Execute

python main.py

or

python src/train_classification.py

or

streamlit run app.py
Libraries Used
Python
Pandas
NumPy
Scikit-learn
XGBoost
LightGBM
SHAP
Matplotlib
Seaborn
Joblib
SciPy
Model Outputs

The project automatically saves:

Reports
Classification Metrics
Regression Metrics
Cross Validation Scores
Feature Importance
SHAP Values
Prediction Results
State Summary
Project Summary
Figures
Correlation Matrix
Feature Importance
SHAP Summary
SHAP Bar Plot
Confusion Matrix
ROC Curve
Precision–Recall Curve
Residual Plot
Actual vs Predicted
Distribution Charts
Models
Best Classification Model
Best Regression Model
Preprocessor
Label Encoder
Applications

This project can support:

Universal Health Coverage monitoring
Health systems strengthening
Resource allocation
Healthcare planning
Public health surveillance
Health financing policy
Healthcare inequality analysis
Decision support systems
Academic research
Data science education
Future Improvements
Integration with official Nigeria DHS and NHMIS datasets
Real-time health dashboard
Interactive GIS visualization
State-level risk forecasting
Time-series monitoring
Deep learning models
Streamlit deployment
Cloud deployment
API integration
Automated reporting

### Author
**Joan Joshua**

### Acknowledgements

This project was developed as an end-to-end public health data science portfolio project demonstrating healthcare analytics, machine learning, and explainable AI for evaluating Universal Health Coverage readiness in Nigeria using synthetic data.

### License

This project is released under the MIT License.
