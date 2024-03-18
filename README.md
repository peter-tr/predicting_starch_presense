# Predicting the Presence of Starch in Food

This project aims to build a machine learning model to predict the presence of starch in various foods based on their nutrient composition. The dataset used in this project was obtained from [Food Standards Australia and New Zealand](https://www.foodstandards.gov.au/science/monitoringnutrients/afcd/Pages/default.aspx).

## Table of Contents
- [Data Pre-processing](#data-pre-processing)
- [Problem Identification](#problem-identification)
- [Modeling Techniques](#modeling-techniques)
  - [K-Nearest Neighbors (KNN)](#k-nearest-neighbors-knn)
  - [Decision Trees](#decision-trees)
  - [Random Forests](#random-forests)
- [Conclusion](#conclusion)
- [Appendix](#appendix)

## Data Pre-processing

The dataset contains information about the nutrient composition of various foods. Initial preprocessing steps included removing columns with low data counts, handling missing values, and eliminating highly correlated features.

Key steps:
- **Removing low data count columns:** Reduced missing data from 60.52% to 0.21%.
- **Correlation Matrix:** Identified and removed highly correlated features to improve model performance.

More details can be found in the full [report](reports/report.md).

## Problem Identification

The goal is to classify foods into two categories: **Starch Present** and **Starch Absent**. The presence of starch was determined based on the nutrient composition of the foods in the dataset.

## Modeling Techniques

### K-Nearest Neighbors (KNN)
A baseline KNN model was first developed, followed by hyperparameter tuning using Grid Search.

### Decision Trees
A decision tree model was built and tuned to handle complex nonlinear relationships in the dataset.

### Random Forests
A Random Forest model was developed to reduce overfitting and improve accuracy. Feature importance was also analyzed.

## Conclusion

The Random Forest model with tuned hyperparameters achieved the highest accuracy of 0.967. This suggests that Random Forests are better suited for this classification problem compared to KNN and Decision Trees. 

## Appendix

For detailed analysis, model comparisons, and code snippets, please refer to the [full report](reports/report.md).

## Running the Project

1. Clone this repository.
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
