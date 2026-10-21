# Predicting Loan Subscription Project - Comparing Boosting Methods 
Here we use the dataset from the UC Irvine Machine Learning Repository (https://archive.ics.uci.edu/dataset/222/bank+marketing)
<img width="1004" height="415" alt="Screenshot 2026-10-21 at 2 23 19 PM" src="https://github.com/user-attachments/assets/e3863752-5f68-4ea3-8d2a-70ddd5592120" />
The marketing campaigns were based on phone calls to new clients.

**AIM**: To determine whether or not a client will subscribe (YES/NO) to a long-term deposit

**Objectives**: 

1) To compare the accuracy of different boosting models in predicting YES/NO, and to determine the optimal model to use for future predictions
   - Models used: RandomForest (baseline), Gradient Boost, Hist-Gradient Boost, LightGBM

2) To determine which client groups to target, based on the features of the clients that did subscribe 

This notebook also walks through using Optuna to tune the hyperparameters of the boosting methods used, and compares the performance of tuned and non-tuned models.

**Project Workflow**
1) Data Extraction
2) Exploratory Data Analysis (EDA)
   - finding unique values
   - finding distribution of target label (identifying class imbalance)
   - finding distributions of numerical variables; counts of categorical variables
3) Data Pre-processing
   - encoding categorical variables
   - handling class imbalance
4) Model Selection + Hyperparameter Tuning/ Optimisation 
   - selecting boosting algorithms
   - hyperparameter tuning and optimisation using Optuna
5) Model Evaluation and Interpretation
   - comparing hyperparameters used
   - visualising ROC scores for each model
   - visualising optimisation history
   - visualising feature importances
   - generating tree diagrams
   - plotting partial dependence plots
   
