# Do You Have Heart Disease?
A machine learning project by Kamri Williams

## Overview
### Research question: “Are you at risk for heart disease?”. 

This project builds and compares machine learning models to predict a patient's likelihood of heart disease based on clinical health metrics."

## Dataset
This data consist of anonymouse patient health data. 

Dataset source: https://www.kaggle.com/datasets/krishujeniya/heartdiseae?

## Tools & Libraries
- **Python** — Primary programming language for data analysis and model development
- **Pandas** — Data manipulation and cleaning, including handling missing values and transforming data
- **NumPy** — Mathematical and array operations
- **Scikit-learn** — Model building, feature scaling, and evaluation metrics
- **Matplotlib & Seaborn** — Data visualization
- **Jupyter Notebook** — Interactive notebook environment for code, visuals, and narrative


## Project Workflow

1. Evaluating & Cleaning the Data —The data was explored for missing values, outliers, and prepared for modeling using pandas functions such as such as .isnull(), StandardScaler, and one-hot encoding.
2. Splitting & Testing the Data — The data was split into 80% training and 20% test sets, with 5 fold cross validation to validate the split.
3. Building the Models — Two models were built to predict heart disease risk: Logistic Regression and KNN.
4. Evaluating the Models — Models were compared using accuracy, precision, recall, and ROC-AUC score.
5. Interpreting the Results — The Logistic Regression model outperformed the KNN model. 

## Results
The Logistic Regression model is better suited for this type of data because the relationship between features like age, cholesterol, and blood pressure and heart disease risk follows predictable, linear patterns.

Performance metrics: 
| Metric | Logistic Regression | KNN |
|--------|-------------------|-----|
| Accuracy | 0.90 | 0.85 |
| Precision | 0.93 | 0.87 |
| Recall | 0.88 | 0.84 |
| ROC-AUC | 0.94 | 0.92 |

![ROC Curve](roc_curve.png)

## Limitation & Future Work
One limitation is that there were no values available for lifestyle factors for individuals. This would have provided a complete picture of the overall health of each individual making a more accurate prediction.
