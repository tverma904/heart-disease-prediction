# Heart Disease Prediction Using Logistic Regression

## Overview

This project uses Logistic Regression to classify records in a heart disease dataset into two target classes. It demonstrates the machine learning workflow, from exploratory data analysis to model training and evaluation.

## Objectives

- Explore and understand the dataset.
- Perform exploratory data analysis (EDA).
- Train a Logistic Regression classification model.
- Evaluate performance using multiple classification metrics.
- Visualize results using a confusion matrix and ROC curve.

## Dataset

The dataset contains **1,025 records and 14 columns**, consisting of 13 input features and one target variable.

The features include age, sex, chest pain type, resting blood pressure, cholesterol, maximum heart rate, exercise-induced angina, and other clinical measurements.

The `target` column represents the two classes used for classification: `0` and `1`.

## Methodology

1. Load and inspect the dataset using Pandas.
2. Examine descriptive statistics, missing values, and target distribution.
3. Separate input features and the target variable.
4. Split the data into training and testing sets using an 80:20 ratio with stratification.
5. Train a Logistic Regression model using Scikit-learn.
6. Evaluate the model on the test set.

## Results

The model achieved the following test-set results:

| Metric | Score |
|---|---:|
| Accuracy | 81.46% |
| Precision | 78.63% |
| Recall | 87.62% |
| F1-score | 82.88% |
| ROC-AUC | 0.8986 |

The test confusion matrix was:

| | Predicted 0 | Predicted 1 |
|---|---:|---:|
| Actual 0 | 75 | 25 |
| Actual 1 | 13 | 92 |

These results describe performance on the particular train-test split used in the experiment. They do not establish clinical diagnostic performance.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## How to Run

1. Open `heart_disease_prediction.ipynb` in Google Colab or Jupyter Notebook.
2. Make the dataset file available in your environment.
3. Update the dataset path if necessary.
4. Run the notebook cells sequentially to reproduce the analysis and evaluation.

## Conclusion

This project demonstrates the use of Logistic Regression for binary classification and illustrates how evaluation metrics and visualizations can be used to assess a machine learning model.

## Limitations

This is an educational machine learning project, not a clinically validated diagnostic system. Its results depend on the dataset, preprocessing, and evaluation procedure used. It must not be used for medical diagnosis or treatment decisions.
