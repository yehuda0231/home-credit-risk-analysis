# Home Credit Risk Analysis

# Project Presentation
https://www.canva.com/design/DAG_hj8gUwQ/0E3g7_XzBi_1fKdcE_r1uA/view?utm_content=DAG_hj8gUwQ&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=he1fd4edfaf

## Project Overview
This project aims to analyze and predict customer credit default risk using machine learning techniques.  
This project was completed as part of the Rakamin Academy Data Science Program in collaboration with Home Credit Indonesia.

Two classification models are used:
- Logistic Regression
- Random Forest Classifier

The final output includes model performance evaluation and business insights derived from feature importance analysis.

---

## Business Problem
Home Credit needs to minimize credit default risk by accurately identifying high-risk customers before loan approval.

Incorrect credit decisions can lead to:
- Increased non-performing loans
- Financial losses
- Reduced business sustainability

---

## Objective
- Build a machine learning model to predict loan default risk
- Compare model performance using ROC AUC
- Identify key factors affecting customer default behavior

---

## Dataset
- Dataset name: **Home Credit Default Risk**
- Source: Kaggle (Home Credit Group)
- Dataset link:  
  https://www.kaggle.com/c/home-credit-default-risk/data

- Main file used:
  - `application_train.csv`
- Rows: ~307,000
- Features: Demographic, financial, and credit-related variables

Target variable:
- `TARGET = 1` → Customer defaulted
- `TARGET = 0` → Customer did not default

> **Note:**  
> The dataset is not included in this repository due to GitHub file size limitations.  
> Please download the dataset directly from the Kaggle link above.

---

## Data Preprocessing
- Selected numeric features only
- Missing values handled using median imputation
- Data split into training (80%) and testing (20%)
- Feature scaling applied for Logistic Regression

---

## Modeling Approach

### Models Used
1. Logistic Regression
2. Random Forest Classifier

### Evaluation Metrics
- Accuracy
- ROC AUC Score
- ROC Curve visualization

---

## Exploratory Data Analysis (EDA)
The following analyses were performed:
- Target distribution analysis
- Age vs default comparison
- Employment length vs default comparison

Visualizations were created to support business interpretation.

---

## Feature Importance
Random Forest feature importance was used to identify key risk drivers.

Top contributing features include:
- EXT_SOURCE_2
- EXT_SOURCE_3
- EXT_SOURCE_1
- DAYS_BIRTH
- DAYS_EMPLOYED

These features significantly influence default prediction.

---

## Results
- Both models achieved ROC AUC above 0.7
- Logistic Regression and Random Forest showed comparable performance
- External credit scores are the strongest indicators of default risk

---

## Conclusion
Machine learning models can effectively support credit risk assessment.  
Feature importance analysis provides valuable business insights for decision-making.

---

## Future Improvements
- Include categorical features with proper encoding
- Apply advanced models (XGBoost, LightGBM)
- Handle class imbalance using resampling techniques
- Perform hyperparameter tuning

---

## Tech Stack
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

## Author
Participant of the Rakamin Academy Data Science Program in collaboration with Home Credit Indonesia



