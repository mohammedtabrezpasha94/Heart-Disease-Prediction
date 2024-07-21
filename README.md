Here's a polished README for your GitHub repository on heart disease prediction using logistic regression:

---

# Heart Disease Prediction using Logistic Regression

## Overview
This project aims to predict the presence of heart disease in patients using logistic regression, a powerful algorithm for binary classification. The dataset used contains features related to heart health, such as age, gender, blood pressure, and cholesterol levels.

## Introduction
Cardiovascular diseases are a leading cause of death globally, with the World Health Organization estimating 12 million deaths annually. Early prediction and diagnosis can significantly improve treatment outcomes and save lives. This project leverages logistic regression to build a predictive model that can identify individuals at risk of heart disease based on health metrics.

## Data Source
The dataset is sourced from an ongoing cardiovascular study on residents of Framingham, Massachusetts. It includes over 4,000 records and 15 attributes, covering demographic, behavioral, and medical risk factors.

## Key Attributes
- **Demographic:** Age, Sex
- **Behavioral:** Current Smoker, Cigarettes Per Day
- **Medical History:** Blood Pressure Medication, Prevalent Stroke, Prevalent Hypertension, Diabetes
- **Medical (Current):** Total Cholesterol, Systolic Blood Pressure, Diastolic Blood Pressure, Body Mass Index, Heart Rate, Glucose Level
- **Target Variable:** 10-year risk of coronary heart disease (CHD)

## Modeling Approach
1. **Exploratory Data Analysis (EDA):** Understanding characteristics and relationships between variables.
2. **Data Preprocessing:** Handling missing values, encoding categorical variables, scaling numerical features.
3. **Logistic Regression:** Training the model with backward elimination for feature selection, removing attributes with the highest P-value until all P-values are less than 0.05.
4. **Model Evaluation:** Using metrics like accuracy, precision, recall, F1-score, and ROC curves.

## Logistic Regression Equations
The logistic regression equation can be expressed as:
\[ P = \frac{e^{\beta_0 + \beta_1X_1}}{1 + e^{\beta_0 + \beta_1X_1}} \]

When all features are included:
\[ \text{logit}(p) = \log\left(\frac{p}{1-p}\right) = \beta_0 + \beta_1 \cdot \text{Sex_male} + \beta_2 \cdot \text{age} + \beta_3 \cdot \text{cigsPerDay} + \beta_4 \cdot \text{totChol} + \beta_5 \cdot \text{sysBP} + \beta_6 \cdot \text{glucose} \]

## Results
- Model achieved an accuracy of 88%.
- Significant predictors include age, sex, cigarettes per day, systolic blood pressure, and glucose levels.
- Men are more susceptible to heart disease than women.
- Increasing age, number of cigarettes smoked per day, and systolic blood pressure increase the odds of heart disease.

## Conclusion
This project demonstrates logistic regression's application in predicting heart disease. Results highlight the importance of various health metrics in determining heart disease risk and provide a foundation for further improvements in healthcare.

## Technologies Used
- **Data Manipulation:** Pandas
- **Data Visualization:** Matplotlib, Seaborn
- **Modeling:** Scikit-Learn

## Link to Project
[GitHub Repository](https://github.com/mohammedtabrezpasha94/heart-disease-prediction)

## Appendix
- [World Health Organization Fact Sheet](http://www.who.int/mediacentre/factsheets/fs317/en/)
- [Data Source](https://www.kaggle.com/amanajmera1/framingham-heart-study-dataset/data)

