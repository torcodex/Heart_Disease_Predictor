Heart Disease Predictor
This project aims to predict the presence of heart disease in a patient based on various medical attributes. The prediction is made using a Logistic Regression model trained on the UCI Heart Disease dataset.

Overview
The primary goal of this project is to build a machine learning model that can accurately identify whether a patient is likely to have heart disease. This is a binary classification problem where the model will predict either the presence (1) or absence (0) of heart disease. The process involves data cleaning, preprocessing, exploratory data analysis (EDA), model training, and evaluation.

Dataset
The project utilizes the Heart Disease UCI dataset, which is a collection of data from four different databases. The dataset contains 14 attributes used for prediction:

age: Age of the patient

sex: Sex of the patient (Male/Female)

cp: Chest pain type (e.g., typical angina, asymptomatic)

trestbps: Resting blood pressure

chol: Serum cholesterol in mg/dl

fbs: Fasting blood sugar > 120 mg/dl (True/False)

restecg: Resting electrocardiographic results

thalach: Maximum heart rate achieved

exang: Exercise-induced angina (Yes/No)

oldpeak: ST depression induced by exercise relative to rest

slope: The slope of the peak exercise ST segment

ca: Number of major vessels (0-3) colored by fluoroscopy

thal: Thalassemia (a blood disorder)

num: The target variable indicating the presence of heart disease (the predicted attribute)

The original dataset is available in heart_disease_uci.csv.

Project Workflow
The project follows a standard machine learning pipeline:

Data Loading and Inspection: The dataset is loaded using Pandas, and an initial inspection is performed to understand its structure and identify missing values.

Data Cleaning & Preprocessing:

Missing values in numerical columns are imputed using the mean of their respective columns.

Categorical features (like sex, cp, thal, etc.) are converted into numerical format using one-hot encoding. This creates binary columns for each category.

Exploratory Data Analysis (EDA): Visualizations are used to understand the relationships between different features and the target variable. A correlation matrix heatmap is generated to see how features are correlated with each other.

Model Training:

The dataset is split into features (X) and the target variable (Y).

The data is further divided into training and testing sets (80% training, 20% testing).

A Logistic Regression model is instantiated and trained on the training data.

Model Evaluation:

The trained model's performance is evaluated on the unseen test data.

Key metrics like Accuracy and the Confusion Matrix are calculated to assess the model's predictive power.

Technologies Used
Python: Core programming language

Pandas: For data manipulation and analysis

NumPy: For numerical operations

Scikit-learn: For machine learning modeling and evaluation

Matplotlib & Seaborn: For data visualization


📊 Results
The Logistic Regression model was trained and evaluated, achieving a solid accuracy score on the test set. The confusion matrix provides a detailed look at the model's performance in terms of true positives, true negatives, false positives, and false negatives, giving insight into its reliability for real-world application.
