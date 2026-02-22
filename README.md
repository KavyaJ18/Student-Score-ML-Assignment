📊 Student Score Prediction using Linear Regression

📌 Project Overview

This project aims to predict students' final exam scores using Machine Learning.
A Linear Regression model is built to understand how study hours, attendance, and previous performance influence academic results.

🎯 Problem Statement

Can we accurately predict a student's final exam score based on:

Study Hours

Attendance Percentage

Previous Exam Score

The goal is to analyze feature importance and evaluate model performance using proper train-test splitting to avoid overfitting.

📂 Dataset Description

A manually created dataset containing 15 samples with the following features:

Feature	Description
Study_Hours	Number of hours studied per day
Attendance	Attendance percentage
Previous_Score	Marks obtained in previous exam
Final_Score	Target variable (final exam score)

The dataset was stored using a Pandas DataFrame.

🔎 Exploratory Data Analysis (EDA)

The following steps were performed:

Checked first and last 5 rows

Verified dataset shape and data types

Checked for missing values

📊 Visualizations Created:

📈 Scatter Plot (Study Hours vs Final Score)

📊 Histogram (Final Score Distribution)

📦 Boxplot (Attendance Distribution)

Key Insight:
A strong positive linear relationship exists between Study Hours and Final Score.

🤖 Model Implementation

Algorithm Used: Linear Regression (Scikit-Learn)

Data Split: 80% Training, 20% Testing

📏 Evaluation Metrics:

Mean Absolute Error (MAE)

R² Score

📊 Model Performance
Model Type	MAE	R² Score
Original Model (3 features)	0.53	0.994
Reduced Model (2 features)	0.33	0.997
Engineered Model (4 features)	0.53	0.993
🔍 Observations

The Reduced Model (Study Hours + Attendance) performed best.

Removing Previous_Score slightly improved performance.

Adding an interaction feature did not significantly improve results.

Simpler models performed better due to the small dataset size.

⚠ Overfitting Check

The model was also trained on the full dataset without a train-test split.

Although R² increased slightly, this evaluation is unreliable because:

The model was tested on the same data it was trained on.

This can lead to overfitting (memorizing rather than generalizing).

Using a train-test split provides a more realistic estimate of model performance.

🧠 Key Learnings

Importance of train-test split

Understanding MAE and R² metrics

Feature importance comparison

Feature engineering experimentation

Overfitting awareness

🛠 Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-Learn

Google Colab

🚀 How to Run

Clone the repository

Open the notebook in Jupyter or Google Colab

Run all cells sequentially

📌 Conclusion

Study Hours and Attendance are the strongest predictors of student performance in this dataset.

This project demonstrates a complete Machine Learning workflow — from data creation and visualization to model training, evaluation, feature comparison, and overfitting analysis.

Now:
