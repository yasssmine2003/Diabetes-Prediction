# Diabetes Prediction using Support Vector Machine (SVM)

## Project Overview

This project uses Machine Learning to predict whether a person is diabetic or non-diabetic based on medical diagnostic measurements. The model is built using the Support Vector Machine (SVM) algorithm and implemented in Python with Scikit-learn.

The project covers the complete machine learning workflow:

* Data loading and exploration
* Data preprocessing and standardization
* Train-test split
* SVM model training
* Model evaluation
* Building a predictive system for new patients

---

## Dataset Information

The project uses the Pima Indians Diabetes Dataset, which contains medical information collected from female patients.

### Features Description

| Feature                  | Description                                   | Impact on Prediction                                                                             |
| ------------------------ | --------------------------------------------- | ------------------------------------------------------------------------------------------------ |
| Pregnancies              | Number of times the patient has been pregnant | Multiple pregnancies may increase the risk of diabetes.                                          |
| Glucose                  | Plasma glucose concentration                  | One of the most important indicators. High glucose levels are strongly associated with diabetes. |
| BloodPressure            | Diastolic blood pressure (mm Hg)              | Abnormal blood pressure may be related to metabolic disorders.                                   |
| SkinThickness            | Triceps skin fold thickness (mm)              | Provides information about body fat distribution.                                                |
| Insulin                  | 2-Hour serum insulin (mu U/ml)                | Helps assess insulin production and resistance.                                                  |
| BMI                      | Body Mass Index                               | Higher BMI often indicates overweight or obesity, which increases diabetes risk.                 |
| DiabetesPedigreeFunction | Genetic predisposition score                  | Measures the likelihood of diabetes based on family history.                                     |
| Age                      | Age of the patient                            | The risk of diabetes generally increases with age.                                               |

### Target Variable

| Value | Meaning      |
| ----- | ------------ |
| 0     | Non-Diabetic |
| 1     | Diabetic     |

---

## Data Preprocessing

Since SVM is sensitive to feature scales, the data was standardized using StandardScaler. This ensures that all features contribute fairly during model training.

---

## Model

The classification model used in this project is:

* Support Vector Machine (SVM)
* Kernel: Linear

The SVM algorithm learns an optimal decision boundary that separates diabetic and non-diabetic patients.

---

## Making Predictions

After training, the model can predict the diabetes status of new patients by:

1. Receiving the patient's medical measurements.
2. Standardizing the input data.
3. Feeding the data into the trained SVM model.
4. Returning a prediction:

   * 0 → Non-Diabetic
   * 1 → Diabetic

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* Support Vector Machine (SVM)

---

## Learning Outcomes

Through this project, I learned:

* Data preprocessing and feature scaling
* Exploratory Data Analysis (EDA)
* Training a Support Vector Machine model
* Evaluating classification performance
* Building a real-world predictive system using Machine Learning
