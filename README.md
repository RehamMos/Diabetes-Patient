# Diabetes-Patient

This dataset is originally from the National Institute of Diabetes and Digestive and Kidney

🌟 The objective of the dataset is to diagnostically predict whether a patient has diabetes.
🌟 Dataset's size is 768 rows, 7 features, and one target. False Negative is the main goal to minimize.

Features Names:
Pregnancies - Glucose - BloodPressure - SkinThickness - Insulin - BMI - DiabetesPedigreeFunction

🌟 After reading the data, EDA shows that the minimum value (zero) can't be the right value of (Glucose, BloodPressure, SkinThickness, Insulin, and BMI) columns, they should be updated with the median value.

🌟 Data is non-linear and there are outliers based on data distribution.
- Measuring correlation between features.
- Splitting data 75% test and 25% train.
- Robust scaler for data scaling.
- Feature selection Information Gain to know which features are the most important for prediction, and they are (Glucose, Age, Pregnancies, Insulin, and BMI).
🌟 Models used for prediction:
- Decision tree with all features and selected features by IG
---- hyperparameter tuning to handle overfitting (min_samples_split, min_samples_leaf).
- KNN with all features and selected features by IG.
- Logistic Regression with all features and selected features by IG
---- hyperparameter tuning to handle overfitting (C)

🌟 Accuracy, Confusion Matrix, and AUC score are used to measure the machine learning models' performance.

🌟 The champion model is Decision Tree with features selected by IG with
Accuracy= 76.5% AUC score=0.747
