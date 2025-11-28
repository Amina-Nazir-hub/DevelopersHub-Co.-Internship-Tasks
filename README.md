# Data Science Internship Projects

This repository showcases solutions for three key data science tasks, demonstrating skills in data analysis, visualization, and machine learning.

## Task 1: Exploring and Visualizing a Simple Dataset (Iris)

### Section	Description
Dataset	Iris Dataset (available via seaborn)  
Skills Used	Pandas for loading/inspection, Matplotlib/Seaborn for visualization.  
### 🎯 Objective
To understand the fundamentals of data handling, summarization, and basic visualization techniques.  
### 💡 Approach
Inspection: Used .shape, .columns, and .head() to examine the dataset structure.  
Visualization: Created key plots to summarize the data:  
Scatter Plots: To analyze relationships between features (e.g., petal length vs. petal width) and species separation.  
Histograms: To show the distribution of individual features (e.g., sepal length).  
Box Plots: To identify outliers and compare spread of values across species.  
### 📊 Results and Insights
**Separation:** Visualizations showed that Setosa is easily distinguishable from other species.  
**Key Features:** Petal Length and Petal Width are the most effective features for classification, with minimal overlap between species.

## Task 2: Customer Churn Prediction (Bank Customers)

### Section	Description  
Dataset	Churn Modelling Dataset (Kaggle)  
Skills Used	One-Hot Encoding, Feature Scaling, Random Forest, Feature Importance Analysis.  
### 🎯 Objective
To build a predictive model to identify high-risk customers likely to leave the bank and analyze factors influencing churn.  
### 💡 Approach  
**Data Preparation:** Removed irrelevant columns and applied Standard Scaling to numerical features.    
**Encoding:** Used One-Hot Encoding for categorical features (Geography, Gender).  
**Modeling:** Trained a Random Forest Classifier with class_weight='balanced' to address class imbalance (~20% churn rate).  
**Evaluation:** Used Accuracy, Classification Report, and Feature Importance analysis.  
### 📊 Results and Insights
**Performance:** Achieved an overall Accuracy of 86.05%, but Recall for churners (1) was 44%, indicating some actual churners were missed.  
**Key Churn Drivers (Feature Importance):**  
Age: Older customers are at higher risk.  
NumOfProducts: Both very low and very high product counts correlate with churn.  
Balance: High balances with low engagement are a warning sign.  
Geography (Germany): Customers in Germany are more likely to leave.  
IsActiveMember: Inactive customers show higher churn risk.  
**Conclusion:** Focus retention strategies on older, inactive customers, particularly in Germany. Future efforts should aim to improve Recall using SMOTE or probability threshold adjustment.

## Task 3: Predicting Insurance Claim Amounts

### Section	Description
Dataset	Insurance Dataset (e.g., from Kaggle)  
Skills Used	Data cleaning, EDA, Regression Modeling (Linear Regression, Random Forest), Evaluation Metrics (MAE, RMSE).  
### 🎯 Objective
To predict the insurance claim amount based on customer demographics, policy details, and risk factors.  
### 💡 Approach
**Data Cleaning:** Handled missing values, corrected inconsistencies, and removed irrelevant columns.  
**EDA:** Visualized relationships between key predictors (e.g., age, BMI, smoking status) and claim amounts.  
**Modeling:** Trained Linear Regression and Random Forest Regressor models.  
**Evaluation:** Measured performance using Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R² Score.  
### 📊 Results and Insights
**Performance:** Random Forest Regressor outperformed Linear Regression with lower MAE and RMSE.  
**Key Predictors:**  
Smoking Status: Smokers tend to have higher claims.  
Age: Older policyholders generally claim more.  
BMI: Higher BMI correlates with higher medical claims.  
**Conclusion:** Insights can help insurance companies set premiums, anticipate high-claim customers, and design risk-based policies.
