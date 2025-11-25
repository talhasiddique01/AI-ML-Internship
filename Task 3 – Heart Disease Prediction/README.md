# Task 3 – Heart Disease Prediction
# Objective
The goal of this task is to build a machine learning model that predicts whether a person is at risk of heart disease based on medical attributes such as age, cholesterol, chest pain type, and exercise-induced angina.
# Dataset Used
1. Heart Disease UCI Dataset (Kaggle)
2. Total Records: 918
3. Target Column: num (converted to binary → 0 = No Disease, 1 = Disease)
4. No missing data
5. Features include:
   1. Age
   2. Sex
   3. Chest Pain Type (cp)
   4. Resting Blood Pressure (trestbps)
   5. Cholesterol (chol)
   6. Fasting Blood Sugar (fbs)
   7. Resting ECG (restecg)
   8. Maximum Heart Rate (thalch)
   9. Exercise-Induced Angina (exang)\
   10. ST Depression (oldpeak)
# Models Applied
  1. Logistic Regression
     1. Standardised all features using StandardScaler
     2. Trained using an 80/20 train-test split
     3. Evaluated using:
        1. Accuracy
        2. Confusion Matrix
        3. ROC Curve + AUC
        4. Classification Report
        5. Feature Importance (model coefficients)
2. Decision Tree Classifier
   1. No scaling required
   2. Evaluated using:
      1. Accuracy
      2. Confusion Matrix
      3. ROC Curve + AUC
      4. Classification Report
      5. Feature Importance (importance)
# Key Results & Findings
Model Performance Comparison 

  | Model                | Accuracy | AUC  |
  |----------------------|----------|------|
  | Logistic Regression  | 0.80     | 0.87 |
  | Decision Tree        | 0.70     | 0.69 |

### Insights from Results
  1. Logistic Regression performed best
     1. With 80% accuracy and AUC=0.87, it clearly identifies high-risk vs low-risk patients.
     2. More stable and generalizes better than the Decision Tree.
  2. The Decision Tree was weaker
     1. Accuracy dropped to 70%, and AUC=0.69, showing poor separation of positive/negative cases.
     2. Slightly overfits due to its structure.
  3. Important Features Identified
     1. From both models, these factors were most strongly associated with heart disease:
        1. thalch (maximum heart rate achieved) — strong negative correlation; lower HR max indicates risk
        2. cp (chest pain type) — certain types strongly indicate heart issues
        3. exang (exercise-induced angina) — presence indicates higher risk
        4. oldpeak (ST depression) — higher values indicate significant abnormality
     2. These medical patterns match real-world clinical indicators.

# Conclusion
  1. Logistic Regression is the best choice for this dataset due to high accuracy and strong ROC-AUC performance.
  2. Key medical indicators like chest pain type, maximum heart rate, and ST depression play a major role in heart disease prediction.
  3. The model can be useful for early screening and risk assessment.

