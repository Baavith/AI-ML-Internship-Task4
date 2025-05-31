# AI-ML-Internship-Task4
❤️ Heart Disease Classification with Logistic Regression
This project builds a binary classification model to predict the presence of heart disease using logistic regression. It follows a complete data science pipeline—from data preprocessing to model evaluation and interpretation.

📂 Dataset
The dataset used is the UCI Heart Disease dataset, where:

num is the original target (0 = no disease, 1–4 = presence of disease).

We convert num into a binary variable:
heart_disease = 1 if num > 0 else 0

✅ Objectives
Predict whether a patient has heart disease.

Evaluate model performance with metrics like confusion matrix, classification report, and ROC-AUC.

Interpret feature contributions using model coefficients.

Experiment with different classification thresholds.

📊 Features Used
The model uses selected numerical features:

age: Age of the patient

trestbps: Resting blood pressure

chol: Serum cholesterol in mg/dl

thalach: Maximum heart rate achieved

oldpeak: ST depression induced by exercise

🧪 Workflow
1. Data Preparation
Load and explore the dataset.

Convert the target variable into binary format.

Handle missing values via mean imputation.

Standardize features using StandardScaler.

Split data into training and test sets (70-30 split).

2. Model Training
Train a logistic regression model on the scaled training data.

3. Evaluation
Generate predictions and probabilities.

Compute:

Confusion matrix

Classification report (precision, recall, F1-score)

ROC curve and AUC score

4. Threshold Tuning
Evaluate performance for thresholds ranging from 0.1 to 0.9 to identify trade-offs between precision and recall.

5. Feature Importance
Analyze feature coefficients to interpret their effect on heart disease prediction.

📈 Results Summary
Sigmoid Function: Used to map linear output to probability.

Thresholding: Default is 0.5, but medical applications may benefit from lower thresholds for higher recall.

Feature Influence: Coefficients indicate which features contribute most to predicting heart disease.

Model Performance: ROC-AUC gives a strong overall view of classifier effectiveness (target: ≥ 0.8)
