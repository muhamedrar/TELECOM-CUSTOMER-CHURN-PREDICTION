# Telco Customer Churn Prediction

## Overview
This project focuses on predicting customer churn for a telecommunications company using machine learning models. Churn is a critical metric for identifying customers likely to stop using the service. The dataset includes demographic and service-related information about customers. The goal is to classify whether a customer will churn or not based on their attributes.

## Dataset
The dataset contains customer information such as:
- Demographic information (gender, age, etc.)
- Service subscription details (Phone, Internet, etc.)
- Account and billing information (Monthly charges, Contract type, Payment method, etc.)

### Features:
- **Categorical Variables**: 
  - Gender, Partner, Dependents, PhoneService, MultipleLines, InternetService, OnlineSecurity, TechSupport, StreamingTV, StreamingMovies, Contract, PaymentMethod, etc.
- **Numerical Variables**: 
  - Tenure, MonthlyCharges, TotalCharges.

## Data Preprocessing
1. Handled missing values.
2. Converted categorical variables to numerical using one-hot encoding.
3. Scaled the numerical features using standardization.

## Model Building
Three models were trained and evaluated:
1. **Logistic Regression**
2. **Decision Tree Classifier**
3. **Random Forest Classifier**

## Performance Comparison

| Model                      | Accuracy  | Precision (Churn) | Recall (Churn) | F1-Score (Churn) |
|-----------------------------|-----------|-------------------|----------------|------------------|
| Logistic Regression          | 85.31%    | 0.85              | 0.84           | 0.85             |
| Decision Tree Classifier     | 81.08%    | 0.88              | 0.81           | 0.84             |
| Random Forest Classifier     | 86.20%    | 0.88              | 0.87           | 0.88             |

- **Logistic Regression**: Achieved a balanced performance with an accuracy of 85.31%.
- **Decision Tree Classifier**: Lower accuracy (81.08%) with slightly reduced recall and F1-scores compared to other models.
- **Random Forest Classifier**: Performed best with an accuracy of 86.20%, showing higher precision and recall for both classes.

## Conclusion
Random Forest provided the best performance in predicting customer churn, with the highest accuracy and balanced metrics. Future improvements could include hyperparameter tuning and experimenting with other ensemble models.
