# PREDICTWISE

1. Overview:
The Student Performance Prediction System is a comprehensive machine learning project designed to help educational institutions, teachers, and students understand and predict academic outcomes. By analyzing various factors such as study habits, attendance, sleep patterns, and facility resources, the system provides actionable insights to improve student success rates.

2. Problem Statement:
Educational institutions face challenges in identifying at-risk students early and providing timely interventions. Traditional methods rely on periodic assessments, which may be too late to prevent academic failures. Additionally, student wellness (physical and mental health) significantly impacts academic performance but is often overlooked.
Key Challenges:

-Early Identification: Detect students at risk of failing before final exams
-Personalized Interventions: Understand individual factors affecting performance
-Holistic Assessment: Consider both academic and health-related factors
-Scalability: Automate predictions for large student populations
-Actionability: Provide clear, interpretable results for educators

3. Project Objectives
This system addresses three critical prediction tasks:
-> Exam Score Prediction (Regression)
Predict a student's final exam score based on:

Age
Daily study hours
Class attendance percentage
Sleep hours
Study method (coaching, self-study, online videos, etc.)
Facility rating (infrastructure quality)

Business Value: Enables proactive academic counseling and resource allocation.

-> Pass/Fail Classification (Binary Classification)
Classify whether a student will pass or fail based on their predicted exam score.
Criteria: Passing score = 50/100
Business Value: Early warning system for at-risk students requiring immediate intervention.

-> Health Status Estimation (Multi-class Classification)
Estimate student health status (Poor, Fair, Good, Excellent) based on:

Age
Sleep hours
Sleep quality
Study hours

Business Value: Identify students experiencing burnout or health issues affecting performance.

4.  Features
Data Preprocessing

- Missing value imputation (median for numerical, mode for categorical)
- Label encoding for categorical variables
- Feature scaling using StandardScaler
- Feature engineering (derived health status metric)
- Train-test split (80-20 ratio)

Model Training

- Multiple algorithm comparison
- Hyperparameter tuning
- Cross-validation ready
- Feature importance analysis

Evaluation

- Regression Metrics: MAE, MSE, RMSE, R²
- Classification Metrics: Accuracy, Precision, Recall, F1-Score, Confusion Matrix
- Comprehensive visualizations
- Model comparison dashboards

Model Persistence

- Joblib serialization for all models
- Saved scalers and encoders
- Metadata export for deployment
- Visualization assets

5. Model Architecture
Algorithms Evaluated
-> Regression Models (Objective 1):

Simple Linear Regression - Baseline model
Polynomial Regression (degree=2) - Captures non-linear relationships
Decision Tree Regressor - Handles complex patterns
Random Forest Regressor SELECTED - Best performance

-> Classification Models (Objectives 2 & 3):

Logistic Regression - Baseline classifier
K-Nearest Neighbors (KNN) - Instance-based learning
Naive Bayes - Probabilistic classifier
Decision Tree Classifier - Interpretable rules
Random Forest Classifier SELECTED - Ensemble superiority
