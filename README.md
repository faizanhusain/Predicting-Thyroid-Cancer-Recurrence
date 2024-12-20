# Predicting-Thyroid-Cancer-Recurrence
The objective of this project is to leverage machine learning techniques to predict the recurrence of thyroid cancer. By analyzing the dataset and identifying key patterns, the project aims to build predictive models that assist in early detection and improve patient outcomes.
# Background:
Thyroid cancer is a significant health concern globally, with recurrence being a critical challenge in treatment and management. Machine learning offers a data-driven approach to identify high-risk patients and optimize care strategies.

## Dataset Overview:
- Rows: 383
- Columns: 17
- Target Variable: Recurred (binary: Yes/No)
- Class Distribution:
  - Recurrence: 108 cases (28.2%)
  - Non-recurrence: 275 cases (71.8%)
## Preprocessing Steps:
 1) Duplicate Removal:
    - Identified and removed duplicate rows to ensure data integrity.
 2) Feature Information:
    - Features like age, gender, smoking history, radiotherapy, and pathology were explored.
    - Recurred is the dependent variable (target).
 3) Missing Values:
    - The dataset includes missing data, handled during preprocessing.
 4) Encoding:
    - Categorical variables like Gender and Pathology were encoded to be model-compatible.
## Model Training and Performance:
1) Model Trained:
   - Logistic Regression
   - Random Forest Classifier
   - Gradient Boosting Classifier
   - Neural Networks
2) Best Performing Model:
   - Random Forest Classifier:
   - Accuracy: 0.95
   - ROC-AUC: 0.91
   - F1-Score: 0.96
3) Insights:
   - Random Forest outperformed other models, making it ideal for this prediction task
   - The feature importance analysis highlighted Risk, T, N, and Pathology as significant predictors of recurrence.
## Performance Insights:
1) Random Forest Classifier:
   - Outperformed other models in terms of accuracy, F1-score, and ROC-AUC.
   - Random Forest identified key predictors like Thyroid Function, Risk, and tumor stage features (e.g., T, N, M) as influential in predicting recurrence.
2) Gradient Boosting Classifier:
   - Achieved comparable performance to Random Forest.
   - Slightly better recall, making it effective for detecting recurrence cases.
3) Logistic Regression:
   - Simpler model with lower performance compared to tree-based models.
   - Struggled with capturing complex relationships in the data.
4) Support Vector Machine (SVM):
   - Good performance on balanced metrics but computationally intensive.
## Impact of Thyroid Function on Performance:
- The Thyroid Function feature, as shown in the count plot, demonstrated that most patients fall into the Euthyroid category.
- However, the imbalance in the target variable (fewer recurrence cases) means models need to prioritize recall to avoid missing positive cases.
- Tree-based models like Random Forest and Gradient Boosting are better equipped to handle such imbalanced data and exploit non-linear relationships between features like Thyroid Function and recurrence.
## Conclusion:
- Random Forest and Gradient Boosting were the top-performing models, achieving high accuracy and ROC-AUC scores.
- These models effectively identified significant features (e.g., Thyroid Function, Risk, and tumor stage) contributing to cancer recurrence prediction.
- Further optimization, such as handling class imbalance and feature engineering, could further improve performance.
