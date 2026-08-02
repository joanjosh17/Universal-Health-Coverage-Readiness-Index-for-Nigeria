# 🏥 Universal Health Coverage Readiness Index in Nigeria

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-2E86C1?style=for-the-badge&logo=xgboost&logoColor=white)
![SHAP](https://img.shields.io/badge/SHAP-Explainable%20AI-8E44AD?style=for-the-badge)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge)

> An end-to-end **public health data science pipeline** that builds a Universal Health Coverage Readiness Index (UHCRI) for Nigeria from ~5,000 synthetic state-level healthcare, demographic, infrastructure, and financing records combining **classification and regression modelling, hyperparameter tuning, and SHAP-based explainability** to reveal which healthcare indicators most influence UHC readiness across Nigerian states.

</div>

---

## 📌 Overview

Universal Health Coverage (UHC) is a global health priority under **Sustainable Development Goal (SDG) 3.8**, ensuring that everyone has access to quality healthcare services without suffering financial hardship.

This project develops a **Universal Health Coverage Readiness Index (UHCRI)** for Nigeria using synthetic healthcare, demographic, infrastructure, and financing indicators. Through advanced data analytics and machine learning, the project evaluates healthcare readiness across Nigerian states, identifies disparities, predicts readiness categories, and provides insights that can support evidence-based health policy and strategic planning.

> **Note:** This project uses a realistic **synthetic dataset** created solely for educational, research, and portfolio purposes.

---

## 🎯 Objectives

- Assess **Universal Health Coverage readiness** across Nigerian states
- Analyse **healthcare infrastructure** and **workforce distribution**
- Measure **healthcare accessibility** and **financial protection**
- Predict **UHC readiness** using machine learning (classification & regression)
- Identify the **most influential healthcare indicators** driving readiness
- Support **evidence-based public health decision-making**
- Demonstrate an **end-to-end public health data science workflow**

---

## 🗂️ Dataset

A realistic **synthetic dataset** of approximately **5,000 observations** representing healthcare indicators across Nigeria — no real patient or facility-level data is used.

### Features

| Feature | Description |
|---------|--------------|
| `Record_ID` | Unique record identifier |
| `State` | Nigerian State |
| `Area_Type` | Urban or Rural |
| `Population` | Estimated population |
| `Health_Facilities` | Number of health facilities |
| `Doctors_per_1000` | Doctors per 1,000 population |
| `Nurses_per_1000` | Nurses per 1,000 population |
| `Insurance_Coverage_pct` | Health insurance coverage (%) |
| `Immunization_Coverage_pct` | Childhood immunization coverage (%) |
| `Skilled_Birth_Attendance_pct` | Skilled birth attendance (%) |
| `Out_of_Pocket_Expenditure_pct` | Household out-of-pocket expenditure (%) |
| `Improved_Water_Access_pct` | Access to improved water (%) |
| `Electricity_Availability_pct` | Health facility electricity availability (%) |
| `Avg_Travel_Time_to_Facility_min` | Average travel time to healthcare facility |
| `UHC_Readiness_Index` | Continuous readiness score (0–100) |
| `Readiness_Category` | Low, Moderate, High |

---

## 🛠️ Tools & Technologies

- **Language:** Python
- **Data Processing:** Pandas, NumPy, SciPy
- **Machine Learning:** Scikit-learn, XGBoost, LightGBM
- **Explainable AI:** SHAP (Summary & Bar plots, global feature importance)
- **Visualisation:** Matplotlib, Seaborn
- **Model Persistence:** Joblib
- **Dashboard:** Streamlit (`app.py`)
- **Hyperparameter Tuning:** RandomizedSearchCV, Stratified K-Fold Cross Validation

---

## ⚙️ Methodology / Project Workflow

```
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
```

1. **Data Cleaning:** Missing value analysis, duplicate detection, and validation of the raw synthetic dataset
2. **Exploratory Data Analysis:** Descriptive statistics, distribution analysis, correlation analysis, boxplots, histograms, pairplots, urban vs rural comparisons, and state-level healthcare summaries
3. **Feature Engineering:** Construction of domain-inspired indicators facilities per 100,000 population, doctor/nurse availability scores, healthcare workforce density, service coverage index, infrastructure index, financial protection index, accessibility index, accessibility risk classification, and insurance level categorisation
4. **Classification Modelling:** Train Logistic Regression, Decision Tree, Random Forest, Gradient Boosting, Extra Trees, and XGBoost to predict `Readiness_Category`
5. **Regression Modelling:** Train Linear Regression, Random Forest Regressor, Gradient Boosting Regressor, and Extra Trees Regressor to predict the continuous `UHC_Readiness_Index`
6. **Hyperparameter Tuning:** Optimise the best-performing models using RandomizedSearchCV with Stratified K-Fold cross-validation
7. **Model Evaluation:** Assess classification and regression models using standard performance metrics and cross-validation scores
8. **Explainable AI:** Apply SHAP to identify the healthcare indicators contributing most to readiness predictions
9. **Prediction System:** Serve the trained classifier/regressor, preprocessor, and label encoder through a prediction pipeline and Streamlit app

---

## 📊 Key Features

- ✅ **Realistic synthetic dataset:** ~5,000 records spanning healthcare infrastructure, workforce, accessibility, and financing indicators across Nigerian states
- ✅ **Comprehensive EDA:** missing value analysis, correlation analysis, distribution plots, and urban vs rural comparisons
- ✅ **Domain-driven feature engineering:** service coverage, infrastructure, financial protection, and accessibility indices
- ✅ **Dual modelling approach:** classification of `Readiness_Category` (Low/Moderate/High) and regression of the continuous `UHC_Readiness_Index`
- ✅ **Six classification models** and **four regression models**, including a hyperparameter-tuned XGBoost classifier
- ✅ **Rigorous tuning:** RandomizedSearchCV with Stratified K-Fold cross-validation
- ✅ **Explainable AI with SHAP:** global feature importance and interpretation of model predictions
- ✅ **Rich visual suite:** correlation heatmaps, feature importance, SHAP plots, confusion matrix, ROC and precision–recall curves, actual vs predicted, and residual plots
- ✅ **State-level insights:** readiness distribution and comparison across Nigerian states
- ✅ **Deployable prediction system:** saved models, preprocessor, and label encoder ready for inference via `app.py`

---

## 📸 Visualisations

The project generates a full suite of exploratory and model-evaluation visuals, including:

- Correlation Heatmap
- Distribution Plots
- State Comparison Charts
- Urban vs Rural Analysis
- Feature Importance
- SHAP Summary Plot
- SHAP Bar Plot
- Confusion Matrix
- ROC Curve
- Precision–Recall Curve
- Actual vs Predicted Plot
- Residual Plot
- Cross-Validation Performance
- UHC Readiness Distribution

---

## 📁 Project Structure

```
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
```

---

## ▶️ How to Run

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/yourusername/Universal-Health-Coverage-Readiness-Index-for-Nigeria.git

# 2. Move into the project directory
cd Universal-Health-Coverage-Readiness-Index-for-Nigeria

# 3. Install dependencies
pip install -r requirements.txt
```

### Running the Project

```bash
python main.py

# or run individual stages
python src/train_classification.py
python src/train_regression.py

# or launch the interactive dashboard
streamlit run app.py
```

**What the pipeline produces automatically:**

| Output | Description |
|--------|--------------|
| Classification & regression metrics | `outputs/reports/` |
| Cross-validation scores | `outputs/reports/` |
| Feature importance & SHAP values | `outputs/reports/`, `outputs/figures/` |
| Prediction results | `outputs/reports/` |
| State summary & project summary | `outputs/reports/` |
| Trained models, preprocessor, label encoder | `models/` |

### Dependencies

```
pandas
numpy
scikit-learn
xgboost
lightgbm
shap
matplotlib
seaborn
joblib
scipy
streamlit
```

---

## 🚀 Applications

This project can support:

- Universal Health Coverage monitoring
- Health systems strengthening
- Resource allocation and healthcare planning
- Public health surveillance
- Health financing policy
- Healthcare inequality analysis
- Decision support systems
- Academic research and data science education

---

## ⚠️ Limitations & Future Work

**Current Limitations:**
- The dataset is **fully synthetic**, so absolute readiness values are illustrative rather than reflective of real state-level conditions
- Indicators are simulated at an **aggregate state level**, without local government area (LGA) or facility-level granularity
- The model does not yet incorporate **temporal dynamics** it represents a single-period snapshot rather than a monitored trend
- **Financial protection and accessibility indices** are proxy constructs and would benefit from validation against real household survey data

**Future Improvements:**
- 🏥 Integration with **official Nigeria DHS and NHMIS datasets** for real-world validation
- 📊 A **real-time health dashboard** for continuous readiness monitoring
- 🗺️ **Interactive GIS visualisation** of state and LGA-level readiness
- 📈 **State-level risk forecasting** and time-series monitoring
- 🤖 **Deep learning models** for richer indicator interactions
- ☁️ **Streamlit and cloud deployment** for public access
- 🔗 **API integration** for downstream health-system applications
- 📝 **Automated reporting** for policy briefs and stakeholder updates

---
<div align="center">

## 👤 Author

**Name:** Joan Joshua

🏥 Public Health Data Scientist | Machine Learning | Explainable AI | Health Systems Analytics

</div>

---

## 📄 License

This project is released under the **MIT License** free to use, adapt, and build upon for research, education, and public health analytics.
See the [LICENSE](LICENSE) file for full details.

---

## 🙌 Acknowledgements

This project was developed as an end-to-end **public health data science portfolio project**, demonstrating healthcare analytics, machine learning, and explainable AI for evaluating Universal Health Coverage readiness in Nigeria using synthetic data.

---

<div align="center">

⭐ **If this project helped you, please consider starring the repo!**

*Part of a broader portfolio of public health data science and machine learning projects focused on health systems strengthening in Nigeria.*

</div>
