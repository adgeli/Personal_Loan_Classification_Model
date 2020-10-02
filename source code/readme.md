# Personal Loan Classification Model

![intro_photo](images/finance-banner.jpg)

*This repository contains Project 2 notebooks and files related to the FinTech bootcamp course at the University of Toronto's School of Continuing Studies.*

---

## Table of Contents

- [Project Objective](#Project-Objectives)
- [Installation Requirements](#Installation-Requirements)
- [Resources and Troubleshooting](#Resources-Troubleshooting )
- [File Contents](#File-Contents)

---

## Project Objectives 

The following project sets to analise and build a model with the objective of predicting the target feature Personal Loan from the dataset [Bank Personal Loan Modeling](resources/Bank_Personal_Loan_Modelling.csv). By fitting a Logistic Regression model, Random Forest model, and XGBoost gradient boosting model, the goal is to create a predictive model. Additionally, the project will compare the results of the three machine learning models through a set of evaluation metrics to measure model performance. Data for the project can be found the [Kaggle](https://www.kaggle.com/itsmesunil/bank-loan-modelling) web site.

![obj_readme.JPG](images/obj_readme.JPG)

### Data Preparation 

First part of the poject conducts an analysis and cleaning of the data in preperation for input into the models.  Data is spit, scaled and oversampling algorithms, Naïve Random Over Sampling (ROS) and Synthetic Minority Oversampling Technique (SMOTE) are applied. After the datasets are prepared, they are exported to be imported into the model notebooks.  Details can be found in the [Data Prep](data_prep.ipynb)

![data_readme.JPG](images/data_readme.JPG)

### Model Analysis 

In the model analysis section of the project, the three models are invesigated to predict Personal Loan and determine feature importance.  Seperate notebooks for each model are prepared for each model investigate.  Machine Learning models analysed are [Linear Regression](logistical_regression.ipynb), [Random Forest](random_forest.ipynb) and [XGBoost](xgboost.ipynb).  After the models have been fitted and compiled, each are export to be upload to the dashboard for findings and analsis presentation.

![model_readme.JPG](images/model_readme.JPG)

### Project Dashboard

The final deliverable summarizes the analysis and findings presented in the data preperation and each of the model analysis notebooks. Of the three models selected to analyse, the model chosen was the XGBoost using the Random Oversample data.  Details on why this model was selected can be found in the  [Summary of Findings](Summary_of_Findings.md) file.  The full project is detail in a [Dash Board](thera_bank_dashboard.ipynb) as final presentation to the client.



![dash_readme.JPG](images/dash_readme.JPG)

---

## Installation Requirements

To successfully view each of the  [Linear Regression](logistical_regression.ipynb), [Random Forest](random_forest.ipynb) and [XGBoost](xgboost.ipynb) models and execute the [Data Prep](data_prep.ipynb), the following installations are required: 

```
pip install xgboost
pip install seaborn
pip install joblib
pip install -U imbalanced-learn
pip instal numpy
pip install matplotlib
pip install hvplot
pip install -U scikit-learn
pip install statsmodels

```
## Resources and Troubleshooting 

[xgboost](https://xgboost.readthedocs.io/en/latest/build.html)    
[seaborn](https://seaborn.pydata.org/installing.html) 
[joblib](https://joblib.readthedocs.io/en/latest/installing.html)     
[imbalanced-learn](https://imbalanced-learn.readthedocs.io/en/stable/install.html)     
[scikit-learn](https://scikit-learn.org/stable/install.html)    
[statsmodels](https://www.statsmodels.org/stable/install.html)  
[Pandas Docs](https://pandas.pydata.org/pandas-docs/stable/getting_started/index.html)      

---

## File Contents

#### Notebooks Order of Execution

- [Data Prep](data_prep.ipynb)
- [Linear Regression](logistical_regression.ipynb)
- [Random Forest](random_forest.ipynb)
- [XGBoost](xgboost.ipynb)
- [Dash Board](thera_bank_dashboard.ipynb)  
- [Summary of Findings](Summary_of_Findings.md)

#### Data Files

- [Bank Personal Loan Modeling](resources/Bank_Personal_Loan_Modelling.csv)
- [Features](resources/features.csv)
- [X test scaled](resources/X_test_scaled.csv)
- [X train scaled](resources/X_train_scaled.csv)
- [X train ROS](resources/X_train_ros.csv)
- [y train ROS](resources/y_train_ros.csv)
- [X train SMOTE](resources/X_train_smote.csv)
- [X train SMOTE](resources/y_train_smote.csv)
- [X train](resources/X_train.csv)
- [X train](resources/y_train.csv)

#### Models
- [Logistic Regression: Scaled Data](models/log_scaled_model.joblib)
- [Logistic Regression: SMOTE Data](models/log_smote_model.joblib)
- [Logistic Regression: ROS Data](models/log_ros_model.joblib)
- [Random Forest: Scaled Data](models/rf_scaled_model.joblib)
- [Random Forest: SMOTE Data](models/rf_smote_model.joblib)
- [Random Forest: ROS Data](models/rf_ros_model.joblib)
- [XGBoost: Scaled Data](models/xgb_scaled_model.joblib)
- [XGBoost: SMOTE Data](models/xgb_smote_model.joblib)
- [XGBoost: ROS Data](models/xgb_ros_model.joblib)

---
