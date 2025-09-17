# Bank Customer Churn Prediction

# 📌 Overview
Customer churn means when customers stop doing business with a company. In banking, churn happens when customers close their accounts or move to another bank.  

This project applies deep learning models (MLP and LSTM) to predict whether a customer will stay (retained) or leave (churned). By identifying churn early, banks can take steps to retain valuable customers.



# Problem Statement
The aim of this project is to:
- Estimate customer churn for a bank.  
- Compare the performance of two deep learning models: Multi-Layer Perceptron (MLP) and Long Short-Term Memory (LSTM).  
- Identify which model works better for churn prediction.  
# Dataset
- Source: [Kaggle - Bank Customer Churn Prediction](https://www.kaggle.com/datasets/bank-customer-churn-prediction)  
- Records: 10,000 customers  
- Distribution:  
  - Retained: 7963 samples  
  - Churned: 2037 samples  
- Features: 14 attributes including CreditScore, Geography, Gender, Age, Balance, NumOfProducts, HasCrCard, IsActiveMember, EstimatedSalary, and Exited.  
# Data Preprocessing
1. Feature Selection – Removed RowNumber, CustomerId, and Surname as they don’t affect churn.  
2. Encoding – Converted categorical values (Gender and Geography) into numerical format.  
3. Class Balancing – Used SMOTE (Synthetic Minority Oversampling Technique) to balance churn vs retained customers.  
4. Feature Scaling – Applied StandardScaler to normalize features.  
5. Data Splitting – Training set: 80%, Testing set: 20%.  
# Models Implemented
# Multi-Layer Perceptron (MLP)
- Input layer, 7 hidden layers, output layer  
- Optimizer: Adam  
- Loss Function: Binary Cross Entropy  
- Regularization: Dropout  
# Long Short-Term Memory (LSTM)
- Input layer, 6 hidden layers, output layer  
- Optimizer: Adam  
- Loss Function: Binary Cross Entropy  
- Regularization: Dropout  
# Model Evaluation
- MLP Accuracy: 88%  
- LSTM Accuracy: 89%  
- Evaluation Metrics: Accuracy, Confusion Matrix, ROC Curve, Classification Report  

# ✅ Conclusion
- Both models successfully predicted customer churn.  
- LSTM slightly outperformed MLP in terms of accuracy.  
- Churn prediction can help banks reduce customer loss by taking proactive measures.  

# 🚀 Future Scope
- Integrate the churn prediction system with CRM platforms for real-time alerts.  
- Implement feedback loops to improve accuracy with new data.  
- Add explainable AI methods (like SHAP or LIME) to interpret predictions.  
