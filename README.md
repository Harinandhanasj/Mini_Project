# Online Shoppers' Purchasing Intention Prediction Using Machine Learning

## 1. Project Overview

Online shopping has become an essential part of modern business. Understanding customers' purchasing behaviour helps e-commerce businesses improve customer experience and increase sales.

This project focuses on predicting whether an online visitor will make a purchase based on their browsing behaviour and website interactions.

The project uses the Online Shoppers Purchasing Intention dataset and applies machine learning classification algorithms to predict purchasing intention.

## 2. Objectives

- To analyse online shoppers' browsing behaviour.
- To identify factors influencing purchasing decisions.
- To perform exploratory data analysis and visualize important patterns.
- To preprocess the dataset for machine learning.
- To build and compare different classification models.
- To identify the most influential features affecting purchasing predictions.

## 3. Dataset Description

**Dataset Name:** Online Shoppers Purchasing Intention Dataset

**Dataset Source:** UCI Machine Learning Repository

**Original Dataset Size:** 12,330 records

**Number of Features:** 17 independent variables

**Target Variable:** Revenue

**Problem Type:** Binary Classification

The dataset contains information about website visitors, including their browsing activities, time spent on different pages, visitor type, traffic information and purchasing behaviour.

The target variable, Revenue, indicates whether a visitor completed a purchase (True) or did not complete a purchase (False).

### Features Used

- Administrative
- Administrative_Duration
- Informational
- Informational_Duration
- ProductRelated
- ProductRelated_Duration
- BounceRates
- ExitRates
- PageValues
- SpecialDay
- Month
- OperatingSystems
- Browser
- Region
- TrafficType
- VisitorType
- Weekend

**Target Variable:** Revenue

## 4. Technologies and Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## 5. Data Cleaning and Preprocessing

The following preprocessing steps were performed:

1. Loaded the dataset using Pandas.
2. Examined the dataset structure and data types.
3. Checked for missing values.
4. Identified and removed 125 duplicate records.
5. Verified that no duplicate records remained.
6. Separated independent and dependent variables.
7. Divided the dataset into training and testing sets using an 80:20 ratio.
8. Applied StandardScaler to numerical features.
9. Applied OneHotEncoder to categorical features.
10. Used SimpleImputer and ColumnTransformer within machine learning pipelines.

After removing duplicate records, the dataset contained 12,205 unique observations.

No missing values were identified in the original dataset.

## 6. Exploratory Data Analysis (EDA)

Exploratory Data Analysis was performed to understand online shoppers' behaviour and identify patterns in the dataset.

The following visualizations were created:

- Purchase Intention Distribution
- Monthly Visitors Distribution
- Purchase Intention Based on Visitor Type
- Weekend versus Weekday Purchasing Behaviour
- Correlation Heatmap

### Key Observations

- Approximately 84.37% of visitors did not complete a purchase, while 15.63% completed a purchase.
- The dataset shows an imbalance between purchasing and non-purchasing visitors.
- Website traffic varies across different months.
- Returning visitors contribute significantly to website visits and completed purchases.
- Weekdays have higher visitor traffic than weekends.
- BounceRates and ExitRates show a strong positive correlation.

## 7. Machine Learning Algorithms

Four classification algorithms were implemented:

### 1. Logistic Regression
A classification algorithm used to estimate the probability of a visitor making a purchase.

### 2. Decision Tree
A tree-based classification algorithm that makes predictions using decision rules.

### 3. Random Forest
An ensemble learning algorithm that combines multiple decision trees to improve prediction performance.

### 4. Gradient Boosting
An ensemble learning algorithm that builds models sequentially to improve prediction accuracy.

## 8. Model Evaluation

The models were evaluated using the following performance metrics:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

### Performance Comparison

| Model | Accuracy | Precision | Recall | F1-score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| Logistic Regression | 84.6% | 50.5% | 79.6% | 61.8% | 91.0% |
| Decision Tree | 85.4% | 53.7% | 49.7% | 51.6% | 70.9% |
| Random Forest | 89.6% | 65.3% | 71.5% | 68.2% | 92.5% |
| Gradient Boosting | 90.2% | 71.1% | 63.6% | 67.1% | 93.6% |

### Best Model

Gradient Boosting achieved the highest accuracy of 90.2%, precision of 71.1% and ROC-AUC of 93.6%.

Random Forest achieved the highest F1-score of 68.2%, while Logistic Regression achieved the highest recall of 79.6%.

Based on the overall evaluation, Gradient Boosting demonstrated the strongest performance in terms of accuracy, precision and ROC-AUC.

## 9. Confusion Matrix Analysis

Confusion matrices were generated to examine the classification performance of all four models.

They provide information about:

- True Positives
- True Negatives
- False Positives
- False Negatives

The results help understand how effectively each model identifies purchasing and non-purchasing visitors.

## 10. Feature Importance Analysis

Feature importance analysis was performed using the Random Forest classifier.

The top influential features identified were:

1. PageValues
2. ExitRates
3. ProductRelated_Duration
4. ProductRelated
5. BounceRates

PageValues was identified as the most important feature, with an importance score of approximately 0.318.

This indicates that browsing behaviour and product-related website interactions contribute significantly to the Random Forest model's purchasing predictions.

## 11. Conclusion

This project demonstrates how machine learning classification algorithms can be used to predict online shoppers' purchasing intention.

Four classification models were developed and evaluated. Gradient Boosting achieved the highest accuracy of 90.2%, while Random Forest achieved the highest F1-score of 68.2%.

Feature importance analysis identified PageValues, ExitRates and ProductRelated_Duration as important features for predicting purchasing intention.

The findings demonstrate how machine learning can help e-commerce businesses understand customer browsing behaviour and improve their understanding of purchasing patterns.

## 12. Project Structure

```text
Online-Shoppers-Purchasing-Intention/
│
├── MINI PROJECT.ipynb
├── online_shoppers_intention.csv
└── README.md
```

## 13. How to Run the Project

1. Clone or download this repository.
2. Install the required Python libraries.
3. Open the Jupyter Notebook.
4. Ensure the dataset is available in the project directory.
5. Update the dataset path if necessary.
6. Run the notebook cells sequentially to reproduce the analysis and model evaluation.

### Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## 14. References

- UCI Machine Learning Repository – Online Shoppers Purchasing Intention Dataset.
- Python Documentation.
- Pandas Documentation.
- Scikit-learn Documentation.

**Project Title:** Online Shoppers' Purchasing Intention Prediction Using Machine Learning

**Project Type:** Machine Learning – Classification
