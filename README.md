# Computational-Statistics
## Stroke Prediction and Risk Analysis using Computational Statistics

## Project Overview
This project utilizes a healthcare dataset to predict the likelihood of stroke occurrence based on demographic, health, and lifestyle factors such as age, gender, hypertension, heart disease, smoking status, BMI, and average glucose level. The analysis involves a complete data science workflow, including data preprocessing, exploratory data analysis, logistic regression modeling, and evaluation of model robustness using cross-validation and bootstrapping. The project aims to provide insights into the most significant factors influencing stroke risk, supporting preventive healthcare strategies and clinical decision-making.

## Dataset
**Source:** World Health Organization (WHO)  
**Attributes:** Age, Gender, Hypertension, Heart Disease, Ever Married, Work Type, Residence Type, Average Glucose Level, BMI, Smoking Status, Stroke Occurrence  
**Objective:** Predict the likelihood of stroke occurrence based on demographic, health, and lifestyle factors.

## Installation and Setup
### Prerequisites
- R (Version >= 4.0)  
- Required Libraries: 
  - dplyr 
  - tidyr 
  - ggplot2 
  - caret 
  - glm 
  - boot 

## Data Preprocessing
- **Handling Missing Values:** Imputation with mean for numerical columns (e.g., BMI, Glucose Level).  
- **Encoding Categorical Variables:** Label encoding for categorical data (Gender, Ever Married, Work Type, etc.).  
- **Feature Scaling:** Standardization of numerical features (Age, Glucose Level, BMI).  
- **Outlier Handling:** Removal of outliers using IQR method.  
- **Data Split:** 80% for training and 20% for testing.

## Exploratory Data Analysis (EDA)
- Correlation Analysis to identify relationships between factors like age, hypertension, heart disease, and stroke occurrence.  
- Visualizations:  
  - **Bar Plot:** Gender vs. Stroke Occurrence  
  - **Box Plot:** Age vs. Stroke Occurrence  
  - **Histograms:** Smoking Status and Stroke Occurrence  
  - **Bar Plot:** Stroke Occurrence by Heart Disease and Hypertension  
  - **Box Plot:** Glucose Level vs. BMI Category with Stroke Occurrence  

## Modeling and Evaluation
### Logistic Regression
- **Purpose:** Estimate the probability of stroke occurrence based on demographics, health, and lifestyle factors.  
- **Metrics Used:** Accuracy, Confusion Matrix, Cross-Validation, and Bootstrapping.  
- **Results:** 
  - Age and Hypertension were identified as significant predictors of stroke occurrence.  
  - Achieved an accuracy of 96% on the test data.  
  - Confusion Matrix revealed a high True Negative rate with minimal False Negatives.  
  - Cross-Validation and Bootstrapping confirmed the model's robustness and stability.

## Results and Conclusions
- Age and Hypertension are the most significant predictors of stroke occurrence.  
- Other factors such as Heart Disease, Glucose Level, and BMI were not statistically significant.  
- The logistic regression model achieved high predictive accuracy, validating its effectiveness in stroke risk analysis.  
- The model is generalizable and performs consistently on unseen data.

## Limitations and Future Work
- **Limitations:**  
  - Lack of detailed lifestyle and health behavior data may limit predictive accuracy.  
  - The model assumes linear relationships between predictors and stroke occurrence.
- **Future Improvements:**  
  - Integrate additional health and lifestyle variables for enhanced model performance.  
  - Explore non-linear models like Random Forest or Gradient Boosting to capture complex interactions.  
  - Implement techniques to handle class imbalance issues for better prediction of minority classes.

## About
Developed as part of the Computational Statistics course to understand the impact of demographic, health, and lifestyle factors on stroke occurrence using data-driven approaches.
