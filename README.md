# Credit Card Customer Attrition Prediction

**End-to-End Machine Learning Project** | Predicting customer churn for a credit card company to support targeted retention strategies.

## 📋 Project Overview
This project develops predictive models to identify customers at high risk of churning from a credit card service. By analyzing customer demographics, relationship variables, transaction behavior, and utilization patterns, the models help the business proactively intervene and reduce costly customer loss.

## 🎯 Business Problem
- Churned customers are significantly more expensive to replace than to retain.
- Goal: Build high-performing classification models to flag at-risk customers early with strong recall/precision balance.

## 🗂️ Dataset
- **Source**: BankChurners.csv (loaded from AWS S3)
- **Target**: `Attrition_Flag` (Existing Customer vs Attrited Customer)
- **Features**: Customer age, gender, education, marital status, income, card category, relationship metrics (months on book, total relationships), transaction activity, credit limit, utilization ratio, etc.

## 🔧 Key Techniques & Models
- **Data Preprocessing**: Data cleaning, feature engineering, one-hot encoding
- **Exploratory Data Analysis**: Visualizations of churn drivers (utilization, transaction count, inactivity, etc.)
- **Modeling**:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - AdaBoost, Gradient Boosting
  - XGBoost, LightGBM, CatBoost
  - KNN, SVM
- **Advanced Techniques**: Recursive Feature Elimination (RFE), hyperparameter tuning, probability cutoffs, precision-recall optimization

## 📊 Results
- Strong performance using ensemble tree-based models (especially XGBoost / LightGBM / CatBoost)
- Focused on business-relevant metrics: **Recall**, **F1-score**, and optimal probability thresholds to catch at-risk customers
- Identified key churn predictors: low transaction activity, high utilization ratio, inactivity periods, and certain demographic segments

## 📄 Reports
- [Full Project Report (PDF)](Reports/Credit%20Card%20Customer%20Attrition%20Report.pdf)
- [Presentation Slides (PDF)](Reports/Credit%20Card%20Customer%20Attrition%20slides.pdf)

## 🛠️ Technologies Used
**Python** • **pandas** • **scikit-learn** • **XGBoost** • **LightGBM** • **CatBoost** • **Matplotlib** • **Seaborn** • **Plotly** • **Optuna** (in some versions)
