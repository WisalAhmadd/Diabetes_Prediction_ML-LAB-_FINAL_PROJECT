🩺 Diabetes Onset Prediction — ML Final Project
Course: BSCS 8th Semester | Machine Learning Lab
Instructor: Saim Sanan
Team Members: Waseem Ahmad & Wisal Ahmad


Project Overview
This project builds a binary classification system to predict whether a patient is likely to develop diabetes based on key medical diagnostic features. Two machine learning models — Logistic Regression and Random Forest — are trained and compared on the Pima Indians Diabetes Database.


Repository Structure
Diabetes-Onset-Prediction/

├── 📓 ML_FINAL_PROJECT.ipynb       ← Main Jupyter Notebook (full code + explanations)

├── 📄 diabetes.csv                 ← Dataset file

├── 📋 proposal.pdf                 ← Project Proposal (PDF)

├── 📝 final_report.pdf             ← Final Report (PDF)

├── 📊 presentation.pptx            ← Presentation Slides

├── 📖 README.md                    ← This file



Dataset
Property	Details
Name	Pima Indians Diabetes Database
Source	UCI Machine Learning Repository / Kaggle
Link	https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database
Rows	768 patient records
Columns	9 (8 features + 1 target)
Target	Outcome (0 = Non-Diabetic, 1 = Diabetic)
Features Used
Feature	Description
Pregnancies	Number of times pregnant
Glucose	Plasma glucose concentration
BloodPressure	Diastolic blood pressure (mm Hg)
SkinThickness	Triceps skin fold thickness (mm)
Insulin	2-hour serum insulin (mu U/ml)
BMI	Body mass index
DiabetesPedigreeFunction	Family history likelihood score
Age	Age of patient (years)



ML Workflow
1. Import Libraries

2. Load & Explore Dataset (EDA)

3. Data Preprocessing

   └── Replace invalid 0s with median values

   └── Check for duplicates

4. Feature Engineering & Visualization

   └── Correlation heatmap

   └── Distribution plots

   └── Boxplots by class

5. Train-Test Split (80/20, stratified)

6. Feature Scaling (StandardScaler)

7. Model 1: Logistic Regression

8. Model 2: Random Forest Classifier

9. Evaluation: Accuracy, F1-Score, ROC-AUC, Confusion Matrix

10. Model Comparison & ROC Curve


Models & Results
Model	Accuracy	ROC-AUC
Logistic Regression	~70–71%	~0.84
Random Forest	~71–72%	~0.86

Exact values depend on random seed and data split.


Technologies Used
Category	Tools
Language	Python 3.x
Environment	Jupyter Notebook / Google Colab
Data	Pandas, NumPy
ML Models	Scikit-learn
Visualization	Matplotlib, Seaborn
Dataset Access	KaggleHub




How to Run
Option A — Google Colab (Recommended)
Upload ML_FINAL_PROJECT.ipynb to colab.research.google.com
Run all cells (Runtime → Run All)
The notebook auto-downloads the dataset via KaggleHub
Option B — Jupyter Notebook (Local)
# 1. Install required libraries

pip install pandas numpy matplotlib seaborn scikit-learn kagglehub

# 2. Launch Jupyter

jupyter notebook ML_FINAL_PROJECT.ipynb

# 3. Place diabetes.csv in the same folder OR use the KaggleHub cell


Installation
pip install pandas numpy matplotlib seaborn scikit-learn kagglehub

Key Findings
Glucose is the strongest predictor of diabetes onset
BMI and Age are also highly significant features
Insulin and SkinThickness had many zero values (invalid) that required preprocessing
Random Forest outperforms Logistic Regression due to non-linear feature relationships
Both models significantly outperform random guessing (AUC > 0.5)


Team
Member	Role
Waseem Ahmad	Data Preprocessing, Model Training
Wisal Ahmad	EDA, Visualization, Evaluation


Submitted for Machine Learning Lab — Final Term Project Assessment
