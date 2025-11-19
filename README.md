# Income Statement Prediction: A Comparative Analysis of Linear and Tree-Based Regression Models
This project uses ML algorithms (Logistic Regression, Random Forest, etc.) to predict $50K+ income from U.S. Census data. We compare baseline and feature-engineered models for best accuracy and insights into key earning factors.

# 📋 Project Overview
This project develops a classification system to predict whether an individual's income exceeds $50,000 annually using demographic and employment data from the U.S. Census Bureau. We implement and compare the performance of multiple machine learning algorithms, including Logistic Regression, Random Forest, Gradient Boosting, XGBoost, and LightGBM.

# 🎯 Objective
The core objective is to systematically evaluate the impact of feature engineering on predictive performance, comparing baseline models with those enhanced by derived attributes to identify the most robust and accurate approach for income classification.


# 📊 Dataset

**1. Source:** U.S. Census Bureau

**2. Samples:** 48,842 instances

**3. Features:** 14 demographic, educational, and employment-related attributes

**4. Target Variable:** Binary classification of income as either "<=50K" or ">50K"

   

# Key Features
**1. Demographic:** age, workclass, race, gender

**2. Educational:** education level, educational-num

**3. Employment:** occupation, hours-per-week

**4. Financial:** capital-gain, capital-loss

# 🛠️ Methodology
Data Preprocessing
Handling missing values represented by "?"

Outlier removal using IQR method (3×IQR)

Log transformation for skewed features

Class imbalance handling

# Feature Engineering
1. Interaction terms (age × hours worked)

2. Derived features (capital net = capital gain - capital loss)

3. Polynomial features (age squared)

4. Multiple encoding strategies (One-Hot, Label, Target encoding)

# Models Implemented
1. Linear Models
   
3. Logistic Regression

# Ridge Classifier

1. Tree-Based Models
   
3. Decision Tree

4. Random Forest

5. Gradient Boosting

6. XGBoost

7. LightGBM

# Evaluation Strategy
80-20 train-test split with stratified sampling

1. Hyperparameter tuning via GridSearchCV with 3-fold cross-validation

2. Performance metrics: Accuracy, Precision, Recall, F1-Score

3. Comparative analysis: Baseline vs Enhanced features

# 📈 Results
Key Findings
Feature Engineering Impact:

**Linear models:** +0.8% average accuracy improvement

**Tree-based models:** -0.1% average accuracy change

Confirmed tree models automatically discover feature interactions

# Best Performing Models:

**Best Linear:** Logistic Regression (82.56% accuracy)

**Best Tree:** LightGBM (87.56% accuracy)

**Accuracy Gap:** 5.0 percentage points in favor of tree models

# Feature Importance:

**Educational level:** strongest correlation with income (r = +0.334)

**Age and hours worked:** moderate positive correlations

**Capital gains:** largest percentage difference between income groups
