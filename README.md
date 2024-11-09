# Wine-Quality-Prediction

## Overview

This project focuses on using machine learning techniques to analyze and predict the quality of red wine based on its physicochemical properties. The dataset provides insights into various features of wine, enabling us to conduct regression analysis, data visualization, and exploratory data analysis (EDA) to uncover relationships between the inputs and the wine's quality score.

## Context

The dataset contains information on the physicochemical characteristics of Portuguese "Vinho Verde" red wine. It was originally curated as part of research by Cortez et al. (2009) and is widely used in machine learning tasks. For convenience, the dataset is also available on Kaggle, but its original source is the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/wine+quality).

Due to privacy considerations, the dataset does not include grape variety, wine brand, or pricing details. Instead, it focuses solely on measurable physicochemical properties and sensory evaluations.

This data can be approached as either a **regression** or **classification** task. Notably, the classes are imbalanced, with more "normal" quality wines than excellent or poor ones.

## Dataset Features

The dataset contains 12 features, with 11 as inputs and one as the output:

### Input Variables (Physicochemical Properties):
1. **Fixed Acidity**  
2. **Volatile Acidity**  
3. **Citric Acid**  
4. **Residual Sugar**  
5. **Chlorides**  
6. **Free Sulfur Dioxide**  
7. **Total Sulfur Dioxide**  
8. **Density**  
9. **pH**  
10. **Sulphates**  
11. **Alcohol**

### Output Variable:
12. **Quality**: A sensory score ranging between 0 and 10.

## Objectives

- Perform exploratory data analysis (EDA) to understand the relationships among variables.
- Build regression models to predict wine quality scores.
- Experiment with classification by setting an arbitrary threshold for quality (e.g., wines with scores ≥7 are "good").
- Evaluate the performance of various models using metrics such as the ROC curve and AUC.

## Approach

### Key Steps
1. **Data Exploration**: 
   - Analyze the dataset to understand distributions, correlations, and outliers.
   - Visualize key trends and relationships using tools like histograms, scatter plots, and correlation matrices.

2. **Feature Engineering**:
   - Create a binary classification label where scores ≥7 are categorized as "good" and the rest as "not good."
   - Eliminate leakage by ensuring the original quality score is not used inappropriately in training.

3. **Model Building**:
   - Perform a train-test split, ensuring stratification where necessary.
   - Experiment with regression algorithms such as Linear Regression, Random Forest, and Gradient Boosting.
   - For classification, use Decision Trees, Logistic Regression, and other classifiers to predict binary labels.

4. **Model Evaluation**:
   - Use appropriate metrics for regression (e.g., RMSE, R²) and classification (e.g., AUC-ROC, precision-recall).
   - Optimize hyperparameters for better performance.

5. **Visualization**:
   - Visualize results and insights through feature importance plots, decision trees, and model performance curves.

## Potential Insights

- Identify which physicochemical features contribute most to high-quality wine.
- Assess the impact of alcohol, acidity, and sulphates on sensory evaluation scores.
- Determine the effectiveness of machine learning models in predicting wine quality.

## Inspiration and Challenges

Beyond simple regression tasks, try converting this into a classification problem by creating a "good" vs. "not good" wine label. Evaluate models using AUC and ROC to practice with hyperparameter tuning and decision tree analysis. This dataset provides an excellent opportunity to practice both regression and classification techniques.

## Acknowledgments

This dataset originates from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/wine+quality). It was shared on Kaggle for ease of access. Special thanks to Cortez et al. (2009) for their contributions to the dataset and the associated research.
