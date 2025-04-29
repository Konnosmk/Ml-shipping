# Dry Docking Cost Prediction using Machine Learning

🚢 Predicting vessel dry-docking costs using Gradient Boosting Regression

---

## Project Overview

This project builds a machine learning model to predict the **dry docking costs** of container ships based on vessel attributes and operational factors.  
The goal is to help shipowners, operators, and finance teams **forecast maintenance costs** more accurately and improve budgeting decisions.

Key techniques used:
- Synthetic but realistic shipping dataset (100 vessels, 3 dry dockings each)
- Feature engineering (vessel size, vessel age, steel market prices)
- Log-transformation to handle skewed cost distributions
- Gradient Boosting Regression with hyperparameter tuning (GridSearchCV)
- Cross-validation evaluation (5-fold CV)

---

## Dataset Description

Each row represents a vessel's dry-docking event and includes:
- Vessel ID
- Year
- Vessel Age (years)
- Docking Number (1st, 2nd, or 3rd docking)
- Vessel Size (TEU)
- Fleet Size
- Region (Asia, Europe, Middle East, North America)
- Steel Price ($/ton)
- Last Dry Dock Cost ($)
- Dry Docking Cost ($) [Target variable]

Cross Features:
- Vessel Age × TEU
- Vessel Size × Steel Price
- Vessel Age × Steel Price

---

## Machine Learning Workflow

- **Data Cleaning**: Remove missing and redundant values
- **Feature Engineering**: One-hot encoding, cross-feature creation
- **Target Engineering**: Log-transformation of Dry Docking Cost and Last Docking Cost
- **Model**: GradientBoostingRegressor
- **Hyperparameter Tuning**: GridSearchCV (81 combinations)
- **Evaluation**: Test Set RMSE and Cross-Validation RMSE
- **Visualization**: Feature Importance and Actual vs Predicted plots

---

## Model Results
| Metric | Value |
|:-------|:------|
| Best Parameters | {'learning_rate': 0.1, 'max_depth': 3, 'min_samples_split': 10, 'n_estimators': 500} |
| Test Set RMSE | **$154,538** |
| Mean Cross-Validation RMSE | **$322,064** |
| Cross-Validation Std Dev | **$132,326** |

---

## Skills Demonstrated

- Data Cleaning and Feature Engineering
- Regression Modeling (Gradient Boosting)
- Hyperparameter Optimization (GridSearchCV)
- Cross-Validation
- Domain Knowledge (Shipping Operations and Finance)

---

##Future Improvements

- Integrate **real historical steel price data** (instead of random generation)
- Model **dockyard effects** (some regions or yards are cheaper/more expensive)
- Predict **time to next dry docking** (not only cost)
- Expand to different vessel types (tankers, bulkers, LNG)
- Try advanced models like **XGBoost** or **LightGBM**
- Implement **SHAP values** for deeper feature interpretation
- Use **time series modeling** if dockings are sequential
- Deploy the model as a **web app** (Streamlit or FastAPI)

---

## 📬 Contact

Feel free to connect on [LinkedIn](https://www.linkedin.com/in/michalopoulos-konstantinos/) or reach out by email to discuss this project further!
