# Diabetes Classification Project with Random Forest

This project aims to build a machine learning model using the **Random Forest** algorithm to classify whether a patient has diabetes or not based on diagnostic data.

### Language & Environment
![Python](https://img.shields.io/badge/Python-3.13.1-blue?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange?logo=jupyter&logoColor=white)

### Tools & Libraries
![Pandas](https://img.shields.io/badge/Pandas-2.2.2-teal?logo=pandas&logoColor=white)
![Numpy](https://img.shields.io/badge/Numpy-2.0.0-purple?logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.9.2-red?logo=plotly&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-0.13.2-lightblue?logo=plotly&logoColor=white)
![ImbalancedLearn](https://img.shields.io/badge/Imbalanced--Learn-0.12.3-yellow?logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1.5.0-green?logo=scikitlearn&logoColor=white)
![Joblib](https://img.shields.io/badge/Joblib-1.4.2-darkblue?logo=python&logoColor=white)

### Model
![RandomForest](https://img.shields.io/badge/Model-RandomForest-yellowgreen)

---

## Project Description

In this project, I carried out several key steps to ensure both data quality and model performance. First, I checked the features that should not contain *NaN* values. The inspection showed that there were indeed no *NaN* values, but some features had `0` values that are not medically valid. To address this, I replaced each `0` value in the affected features with the **median** of that feature. After cleaning the data, I examined the class distribution in the target variable `Outcome` and found an imbalance, where the number of non-diabetic patients was much higher than diabetic patients. To mitigate this imbalance and avoid model bias toward the majority class, I applied the **SMOTE (Synthetic Minority Oversampling Technique)** method, which generated additional samples for the minority class and made the dataset more balanced. With clean and balanced data, I then built and trained a **Random Forest Classifier** to predict the likelihood of a patient having diabetes.
