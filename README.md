# Telecom Marketing Campaign Prediction

 This project focuses on predicting whether a customer will subscribe to a new telecom plan based on past campaign interactions and customer attributes. It demonstrates a full data science workflow, from data exploration through feature engineering, model selection, and evaluation.

## Project Overview 
The dataset includes customer information, interaction history, and results of past marketing campaigns.
The business goal is to identify customers with a high likelihood of subscribing to reduce campaign costs and improve efficiency.

## Technologies & Tools
Python: Pandas, NumPy, Scikit-learn

Visualization: Matplotlib, Seaborn

Machine Learning: Logistic Regression, SVM, Decision Trees, Random Forest

Model Tuning: GridSearchCV, K-Fold Cross Validation

## Workflow
### 1. Exploratory Data Analysis (EDA)
  
  Generated descriptive statistics for numerical features.
  
  Summarized categorical distributions (e.g., job type, marital status, education).
  
  Unified inconsistent category formats (e.g., multiple labels for same meaning).
  
  Counted missing values and analyzed their patterns.
  
  Conducted correlation analysis across features.
  
  Visualized feature distributions and relationships to target variable.
  
### 2. Data Preprocessing
  
  Converted categorical variables into binary features (one-hot encoding).
  
  Defined and treated outliers using the Interquartile Range (IQR) method, replacing extreme values with threshold limits.
  
  Removed rows with more than 3 missing values.
  
  Normalized features with MinMaxScaler to standardize input for models.
  
  Identified and removed duplicate/redundant columns.
  
  Dropped index columns irrelevant to prediction.
  
  Applied feature selection to reduce dimensionality and improve model efficiency.
  
### 3. Modeling
  
  Goal: maximize AUC score.
  
  Trained and compared multiple algorithms:
  
  Logistic Regression
  
  Support Vector Machine (SVM)
  
  Decision Tree
  
  Random Forest
  
  Applied Grid Search for hyperparameter tuning.
  
  Selected SVM as the best performing model, restricted to the top 25 features.
  
### 4. Model Evaluation
  
  Generated Confusion Matrix for classification results.
  
  Plotted ROC curves for each K-Fold cross-validation run.
  
  Compared train vs. validation results to check for overfitting.
  
  Ensured model robustness before applying to test data.
  
### 5. Final Prediction
  
  Applied same preprocessing steps to the test set.
  
  Ran final predictions with optimized SVM model.

  Exported results into a CSV file for submission.


## Key Results
  Best model: Support Vector Machine (SVM) with tuned hyperparameters.
  
  Achieved strong AUC score 73.5%, indicating reliable classification performance.
