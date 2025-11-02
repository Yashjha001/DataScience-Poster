🎓 MOOC Dropout Prediction using Logistic Regression
📘 Overview

This project predicts student dropout probability in Massive Open Online Courses (MOOCs) using an interpretable Logistic Regression model.
It leverages the Open University Learning Analytics Dataset (OULAD) to analyze learner engagement, demographics, and performance, providing actionable insights to improve course retention.

🎯 Objectives

Predict whether a learner will drop out before course completion.

Identify key behavioral factors influencing dropout.

Categorize learners into Low, Medium, and High-risk tiers.

Recommend targeted interventions (reminders, mentorship, support).

🧩 Dataset

Source: Open University Learning Analytics Dataset (OULAD)

Key Features:

age_band, gender, highest_education, studied_credits

logins_per_week, avg_session_time, assignments_submitted, forum_posts

Derived: engagement_score, early_submission_rate, days_inactive_first2weeks

Target Variable: dropout_status (0 = Continue, 1 = Dropout)

⚙️ Methodology

Data Preprocessing: Handle missing values, encode categories, scale numerical features.

Exploratory Data Analysis: Identify patterns and correlations in student engagement.

Modeling: Train Logistic Regression with class_weight='balanced'.

Evaluation: Assess using ROC-AUC, F1, Recall, and Confusion Matrix.

Interpretation: Analyze feature coefficients to understand dropout causes.

Intervention: Categorize students into risk tiers for targeted support.

📈 Results

Accuracy: 0.84

ROC-AUC: 0.87

Recall (Dropout): 0.82

Key Predictors: assignments_submitted, logins_per_week, days_to_first_login, forum_posts.

💡 Insights & Interventions

Early engagement = higher completion rates.

Automate reminders for medium-risk learners.

Provide mentor guidance for high-risk learners.

Helps institutions reduce dropout and boost retention.

🧠 Tech Stack

Python, Jupyter Notebook

Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn

🧾 Project Structure
📂 MOOC_Dropout_Prediction
 ├── data/
 │   └── anonymisedData.csv
 ├── notebooks/
 │   └── model_training.ipynb
 ├── results/
 │   ├── roc_curve.png
 │   ├── confusion_matrix.png
 │   └── feature_importance.png
 ├── README.md
 ├── requirements.txt
 └── app/
     └── dashboard.py (optional Streamlit/Flask)

👥 Team

Yash Jha – Problem Definition & Model Design

Avadh – Literature Review & Validation

Param & Shubham – Research & Content

Mansoor & Harsh – Poster & Visualization

🏁 Conclusion

An interpretable, lightweight Logistic Regression model that predicts learner dropouts early and supports personalized, low-cost interventions to improve MOOC completion rates.

