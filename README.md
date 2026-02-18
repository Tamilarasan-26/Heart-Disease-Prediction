Heart Disease Prediction – Data Analysis & Machine Learning Report
Project Name: Heart Disease Prediction
 Domain: Healthcare
 Prepared By: Tamilarasan M
 Course: Data Science
 Date: February 2026

1. Introduction
Cardiovascular diseases are one of the leading causes of death worldwide. Early detection plays a crucial role in preventing severe health complications and reducing mortality rates. This project focuses on analyzing patient health data and building a predictive machine learning model to identify individuals at risk of heart disease.

2. Problem Statement
The objective of this project is to analyze patient health records and develop a machine learning model to predict whether a person is likely to have heart disease based on clinical and medical features.

3. Dataset Description
Total number of records: 180


Total number of features: 13 input features + 1 target variable


Target variable: Heart Disease


0 = No Heart Disease


1 = Heart Disease


Feature Types
Numerical Features:
Age


Resting Blood Pressure


Serum Cholesterol


Maximum Heart Rate Achieved


ST Depression (Oldpeak)


Categorical Features:
Sex


Chest Pain Type


Fasting Blood Sugar


Resting ECG Results


Exercise Induced Angina


Slope of ST Segment


Number of Major Vessels


Thalassemia


Description of Key Features
Age: Age of the patient in years


Sex: Gender of the patient (0 = Female, 1 = Male)


Chest Pain Type: Type of chest discomfort experienced


Blood Pressure: Resting blood pressure (mm Hg)


Cholesterol: Serum cholesterol level (mg/dl)


Maximum Heart Rate: Maximum heart rate achieved during exercise


Oldpeak: ST depression induced by exercise



4. Data Preprocessing
4.1 Data Cleaning
No significant missing values found


Duplicate records were checked and removed if present


Data types were verified and corrected


4.2 Outlier Detection
Boxplot analysis was performed


IQR method used for identifying extreme outliers


4.3 Encoding Categorical Variables
Label Encoding applied for ordinal categories


One-Hot Encoding applied where necessary


4.4 Feature Scaling
StandardScaler used for scaling numerical features


Scaling applied after train-test split to avoid data leakage



5. Exploratory Data Analysis (EDA)
5.1 Univariate Analysis
Age distribution shows most patients between 45–65 years


Cholesterol shows slight right skew


Target variable moderately balanced


5.2 Bivariate Analysis
Higher age associated with increased heart disease risk


Higher ST depression strongly linked to heart disease


Lower maximum heart rate associated with disease presence


Chest pain type and number of vessels show strong association


5.3 Correlation Analysis
Oldpeak positively correlated with heart disease


Maximum heart rate negatively correlated


Age moderately correlated


Key Insights:
ST depression and chest pain type are strong predictors


Exercise-induced angina increases risk


Fasting blood sugar has minimal impact



6. Model Building
6.1 Train-Test Split
Train size: 75%


Test size: 25%


6.2 Models Used
Logistic Regression


Decision Tree


Random Forest


Hyperparameter tuning was performed for tree-based models.

7. Model Evaluation
Evaluation Metrics Used:
Accuracy


Precision


Recall


F1-Score


Confusion Matrix


ROC-AUC Score


Logistic Regression (Best Model)
Accuracy: 84%


Recall: 73%


F1-Score: 0.84


AUC Score: 0.88


Cross-validation Recall: 75%


Decision Tree (Tuned)
Accuracy: 80%


Recall: 69%


Random Forest (Tuned)
Accuracy: 84%


Recall: 73%



Best Performing Model: Logistic Regression
Reason:
Highest AUC Score (0.88)


Stable cross-validation performance


Good balance between accuracy and recall


No significant overfitting


Highly interpretable (important in healthcare)



8. Feature Importance
Top important features:
Oldpeak (ST Depression)


Chest Pain Type


Number of Major Vessels


Maximum Heart Rate


Age


Interpretation:
Higher ST depression significantly increases heart disease risk.


Lower maximum heart rate is associated with higher disease probability.


Certain chest pain types strongly indicate heart conditions.



9. Business / Hospital Recommendations
Based on model findings:
High-risk patients should undergo regular cardiovascular screening.


Patients with high cholesterol and high blood pressure should receive preventive care.


Individuals showing high ST depression should receive immediate evaluation.


Lifestyle modification programs (diet, exercise, smoking cessation) should be implemented.


Early intervention strategies can significantly reduce mortality rates.



10. Conclusion
This project successfully analyzed healthcare data and developed a machine learning model to predict heart disease risk. Logistic Regression was selected as the final model due to its strong predictive performance (84% accuracy, 0.88 AUC) and good generalization ability.
The model demonstrates that key clinical factors such as ST depression, chest pain type, and maximum heart rate are strong indicators of heart disease.
This predictive system can assist healthcare providers in early risk detection, enabling timely medical intervention and improving patient outcomes while maintaining interpretability and reliability.
