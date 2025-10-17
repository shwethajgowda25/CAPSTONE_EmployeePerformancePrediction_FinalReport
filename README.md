# **Identifying the Best Classifier: Gradient Boosting for Employee Performance**

<img width="1024" height="1024" alt="EmployeePerformancePrediction_Image" src="https://github.com/user-attachments/assets/f4fc0853-868f-49e8-87bc-b58a6d4b1bd4" />

# Inital EDA Link
https://github.com/shwethajgowda25/CAPSTONE-EmployeePerformancePrediction-Project

# **🏆 Final Model Comparison and Performance Analysis**
This report summarizes the results of the machine learning phase for the Employee Performance Prediction project. Three classification models—Random Forest, Gradient Boosting, and Support Vector Machine (SVM)—were trained, evaluated, and compared using the preprocessed employee dataset.

# **📊 Summary of Model Performance**
The models were evaluated based on Accuracy, which measures the proportion of correctly classified instances across all performance ratings (2, 3, and 4).

<img width="1700" height="308" alt="image" src="https://github.com/user-attachments/assets/b372da06-812f-49ad-9708-0e76cf14095d" />

Visual Comparison of Accuracy

# **🎯 What Model Works Best for the Given Dataset?**

The Gradient Boosting Classifier is the best-performing model for predicting employee performance based on this dataset, achieving the highest accuracy of 92.78%.

While Random Forest performed nearly identically at 92.50%, Gradient Boosting showed slightly superior overall metrics, indicating a marginal edge in generalization and predictive power. The SVM model, despite using standardized data, lagged significantly behind the ensemble methods.

# **🔍 Detailed Model Scoring Analysis**

The detailed performance metrics (Precision, Recall, F1-Score) provide a deeper understanding of how well each model predicts the different performance rating classes (2: Good, 3: Excellent, 4: Outstanding).

# 1. Gradient Boosting Classifier (Best Model)
<img width="1480" height="376" alt="image" src="https://github.com/user-attachments/assets/c00ec4ef-9006-483d-a633-b9ca28f08e31" />

**Analysis:**

High F1-Scores across all classes demonstrate excellent balance between Precision and Recall.

The model is highly effective at identifying the Outstanding (4) employees, with a Precision of nearly 95%, meaning that when it predicts an employee is Outstanding, it is almost always correct.

It shows the best balance for predicting the majority classes (2 and 3).

# 2. Random Forest Classifier (Strong Performer)
<img width="1204" height="382" alt="image" src="https://github.com/user-attachments/assets/d896c317-9501-4b33-b944-b1f971661844" />

**Analysis:**

Performance is very close to Gradient Boosting.

It has the highest Precision for class 4 (Outstanding), indicating high confidence when predicting this top tier.

# 3.  Support Vector Machine (SVM) Classifier (Subpar Performance)
<img width="1206" height="388" alt="image" src="https://github.com/user-attachments/assets/ab03a617-e76b-4bef-9767-8f0bcda08c19" />

**Analysis:**

The SVM struggled significantly with Class 4 (Outstanding), correctly identifying only 16.67% of the true Outstanding employees (low Recall). Although its precision for this class is 1.0 (meaning every prediction of '4' was correct), its failure to find most of them makes it an unreliable predictor for the highest performers.

This model is not suitable for deployment in its current form.

# **🚀 Conclusion and Recommendation**
**Recommendation: Deploy the Gradient Boosting Classifier model.**
While both ensemble models performed exceptionally well, Gradient Boosting provided the most consistent high-level performance across all evaluation metrics and classes. Its robust prediction of high-performing employees (Class 4) is critical for strategic human resources planning.

**Next Steps:**
**1. Hyperparameter Tuning**: Further optimize the Gradient Boosting model using techniques like Grid Search or Randomized Search to potentially push the accuracy above 93%.

**2. Feature Importance**: Extract and analyze feature importance from the Gradient Boosting model to gain final, actionable insights on what drives employee performance.

