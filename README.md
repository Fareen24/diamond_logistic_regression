# Diamond Cut Prediction
This repository contains an analysis and machine learning model to predict the cut of a diamond based on various features such as carat, color, clarity, depth, table, price, and dimensions (x, y, z). The dataset used in this project includes multiple features related to diamonds and their physical properties.


## Project Overview
The primary goal of this project is to predict the cut of a diamond (with categories such as Ideal, Premium, Good, Very Good, Fair) using a logistic regression classifier. Various steps are undertaken in this project, from data cleaning and outlier removal to model building and performance evaluation.

# Key Features:
**Data Preprocessing**: Outlier removal using the Interquartile Range (IQR) method.

**Modeling**: Multinomial Logistic Regression for predicting diamond cut.

**Evaluation**: Confusion matrix, classification report, accuracy score, and F1-score metrics are used to evaluate the performance of the model.

**Visualization**: Includes visualizations like confusion matrix heatmaps to interpret model performance.

# Dataset
The dataset includes the following columns:

**carat**: Weight of the diamond.

**cut**: Quality of the diamond cut (target variable) — Ideal, Premium, Good, Very Good, Fair.

**color**: Diamond color (ranging from D, E, F, G, H, I, J).

**clarity**: Diamond clarity (ranging from I1, SI1, SI2, VS1, VS2, VVS1, VVS2, IF).

**depth**: Total depth percentage.

**table**: Width of the top of the diamond relative to its widest point.

**price*8: Price of the diamond.

**x, y, z**: Dimensions of the diamond.

# Steps taken:
## 1. Loading necessary libraries and data:
Imported the necessary libraries and loaded the dataset into a pandas Dataframe.

## 2. Exploratory Data Analysis:
Visualized distributions of key features.
Analyzed relationships between features and the target variable cut.
## 3. Modeling:
Multinomial Logistic Regression was used to model the relationship between diamond features and the cut category.
Cross-validation was applied to evaluate model performance.
## 4. Evaluation:
Confusion Matrix: Visualized using Seaborn heatmap.

Classification Report: Precision, Recall, F1-Score for each cut category.

Accuracy Score: Evaluated overall accuracy of the model.

# Results
The model achieved an accuracy score of 69%.

Performance varies across different diamond cut categories, with the highest F1-scores for the Good and Very Good cuts.

The confusion matrix shows areas of misclassification, particularly between Premium and Good cuts.