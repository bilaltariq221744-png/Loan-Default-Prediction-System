# Loan Approval Prediction using Machine Learning

## Project Overview

This project aims to build a machine learning model to predict whether a loan application will be approved or rejected based on an applicant’s financial and demographic information. The dataset contains approximately 4,200 loan records with features such as income, loan amount, CIBIL score, asset values, employment status, and education level.

The dataset was imbalanced, with a higher proportion of approved loans than rejected ones. To address this issue, SMOTE (Synthetic Minority Oversampling Technique) was applied to balance the training data. Two classification models, Logistic Regression and Decision Tree, were implemented and compared to evaluate their performance.

---

## Dataset Description

The dataset includes multiple financial and personal attributes of loan applicants, including number of dependents, annual income, loan term, credit score, and different categories of assets. The target variable, `loan_status`, indicates whether the loan was approved or rejected.

Initial analysis revealed class imbalance in the dataset, which required appropriate handling to avoid biased model predictions.

---

## Data Preprocessing and Exploration

Data preprocessing involved cleaning column names, removing inconsistencies, handling missing values, encoding categorical variables, and preparing the dataset for modeling.

Exploratory Data Analysis (EDA) was conducted to understand feature distributions and their relationships with the target variable. Correlation analysis and visualizations were used to identify important factors influencing loan approval decisions.

---

## Handling Class Imbalance

Due to the uneven distribution of approved and rejected loans, SMOTE was applied to the training dataset to generate synthetic samples for the minority class. This improved the model’s ability to learn patterns from both classes and enhanced overall prediction performance.

---

## Model Development

Two classification algorithms were implemented:

- **Logistic Regression**, which models linear relationships between features and the target variable.
- **Decision Tree**, which captures non-linear relationships and feature interactions.

Both models were trained on the balanced dataset and evaluated using multiple performance metrics.

---

## Model Evaluation and Results

Model performance was evaluated using Accuracy, Precision, Recall, F1-score, and Confusion Matrix. Since the dataset was imbalanced, greater importance was given to precision, recall, and F1-score rather than relying solely on accuracy.

The Decision Tree model outperformed Logistic Regression in terms of precision, recall, and F1-score, indicating better performance in correctly classifying both approved and rejected loan applications.

---

## Technologies Used

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- Imbalanced-learn (SMOTE)  

---

## Key Takeaways

This project demonstrates the importance of proper data preprocessing, handling class imbalance, and selecting suitable evaluation metrics in classification problems. It also highlights how different algorithms can produce varying results depending on the structure and characteristics of the dataset.

---

## Future Improvements

Future work may include hyperparameter tuning, cross-validation for improved generalization, experimentation with ensemble models such as Random Forest or Gradient Boosting, and deployment of the model as a web application.

---

## Author

Bilal Tariq
