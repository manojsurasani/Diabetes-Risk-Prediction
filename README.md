# Diabetes Risk Prediction 🩺📊

## Overview
The goal of this project is to predict the risk of diabetes based on patient data, including demographics, medical history, and lifestyle factors. 

## Dataset
The dataset utilized in this project is `framingham.csv'. It contains 4,240 records of individuals with 16 features relevant to diabetes risk assessment. Key features analyzed include age, education, smoking habits, cholesterol levels, blood pressure, BMI, heart rate, and glucose levels.

## Project Workflow
1. **Data Exploration:** The dataset is loaded and examined for missing values, and the key distribution of the diabetes risk target variable is visualized.
2. **Data Preprocessing:** The data is cleaned by dropping unnecessary columns (like `TenYearCHD`), handling missing values by substituting them with the median, and normalizing numerical features using `StandardScaler`.
3. **Model Training:** A Logistic Regression classification model with balanced class weights is trained to predict the risk of diabetes.
4. **Evaluation:** The model's performance is assessed using accuracy metrics and a detailed classification report.

## Tech Stack
* **Language:** Python
* **Data Manipulation & Analysis:** pandas, NumPy
* **Machine Learning:** scikit-learn (Logistic Regression, StandardScaler, train_test_split)
* **Visualization:** matplotlib, seaborn

## Results
* The Logistic Regression model achieved an overall accuracy of **0.9186** (approximately 92%) on the testing dataset.
* The classification report highlights a strong ability to identify non-diabetic cases (precision of 0.99), alongside a recall of 0.82 for positive diabetic cases.
