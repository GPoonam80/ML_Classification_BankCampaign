# ML_Classification_BankCampaign
# 📊 Bank Marketing Campaign Analysis - Machine Learning Project

![bank](https://github.com/user-attachments/assets/57f969f1-c40c-48b2-b4ce-72c72154486c)

## 🎯 Objective

Develop a classification model to predict whether a customer will subscribe to a deposit scheme based on various demographic and financial factors. This involves data cleaning, exploratory data analysis (EDA), feature engineering, and model building.

## 📊 Data Understanding & Preprocessing

 ### 1️⃣ Dataset Overview

              -  Rows: 11,162
                
              -  Columns: 17
                
              -  Target Column: deposit (Categorical: Yes/No)
                
              -  Balance Distribution: Positively skewed
                
              -  Duplicates & Missing Values: None found ✅
                
              -  Problem Type: Classification

          

### 2️⃣ Data Cleaning

          -  Dropped Redundant Columns: contact, day, month (no significant impact on target)

          -  Categorical Features Grouping:

                -- Job Categories: Merged similar roles to avoid high dimensionality

                -- Education Categories: Merged unknown into tertiary

                -- Poutcome Categories: Simplified into fewer meaningful groups

        -  Handled Outliers:

               -- pdays: Replaced -1 with a high unrealistic number to maintain business meaning, then applied reciprocal transformation

### 3️⃣ Feature Encoding

        -  One-Hot Encoding: job

        -  Label Encoding: marital, default, housing, loan, poutcome, deposit

        -  Ordinal Encoding: education

        -  Feature Scaling: Standardization applied to numerical features

### 🔍 Exploratory Data Analysis (EDA) & Key Insights

        -  Impact of duration on deposit: Longer call duration correlates with higher subscription probability 📞✅

        -  Boxplots & Countplots:

            -- balance & duration show a strong relationship with deposit

            -- day and contact had minimal impact and were dropped

            -- month distribution varied, but removing it reduced dataset dimensionality for better model efficiency

### 🏗️ Model Building & Evaluation

### 🔬 Train-Test Split (80-20%)

      -  Target variable balanced, so no resampling needed ✅

### 🏆 Model Comparison

      -  Evaluated multiple models using accuracy, precision, recall, F1-score, and confusion matrix:

### Random Forest performed best 🎯

### Overfitting detected: Train score significantly higher than test score 🔴

### 🔧 Model Optimization

      -  Hyperparameter Tuning to reduce overfitting

      -  Cross-Validation for more reliable performance estimation

## 🚀 Key Takeaways

**Data Cleaning & Preprocessing:** Handling categorical variables efficiently to prevent high dimensionality

**Feature Engineering:** Identified impactful variables (balance, duration) and removed redundant ones (day, contact, month)

**Model Evaluation:** Random Forest performed best, but tuning was required to avoid overfitting

**Skills Demonstrated:** Data Wrangling, EDA, Feature Engineering, Classification Models, Hyperparameter Tuning, Model Evaluation

**📍Next Steps:** Improve model generalization and deploy for real-world application.






