# Wine Quality Prediction

## Introduction

This project focuses on predicting the quality of red and white vinho verde wine samples from the north of Portugal. The goal is to model wine quality based on physicochemical tests. The quality levels range from 0 to 10. The models used K-Nearest Neighbors.

## Data Visualization

The datasets were initially visualized using bar plots and correlation matrices to understand the distribution of data and the relationships between different features.

## Data Preprocessing

The wine quality was categorized into two categories: 'low' (0-5) and 'high' (6-10). This transformed the multi-class problem into a binary classification problem. Label Encoding was then applied to convert these categorical labels into numerical form.

## Model Training and Evaluation

A K-Nearest Neighbors (KNN) classifier was trained on the red and white wine datasets separately. The performance of the models was evaluated using various metrics like accuracy, precision, recall, and f1-score.

For the red wine dataset, the baseline KNN model achieved an accuracy of 75%. After hyperparameter tuning, the accuracy increased to 82%. The cross-validation scores ranged from 0.8242 to 0.8633 with a mean score of 0.8444.

For the white wine dataset, the baseline KNN model achieved an accuracy of 38%. After hyperparameter tuning, the accuracy increased to 83%. The cross-validation scores ranged from 0.7908 to 0.8214 with a mean score of 0.8060.

## Conclusion

The hyperparameter-tuned KNN models demonstrated superior performance compared to the baseline models in predicting the quality category of both red and white wines. This project is a good example of how machine learning can be applied to solve classification problems in the wine industry. Future work could explore other machine learning models and feature engineering techniques to further improve the prediction accuracy.

## Recommendations

Based on the analysis, the Random Forest model is recommended for predicting wine quality due to its superior performance. However, it's important to keep in mind the limitations of the analysis and the potential improvements for future work.

## Reference:

Cortez, P., Cerdeira, A., Almeida, F., Matos, T., & Reis, J. (2009). Modeling wine preferences by data mining from physicochemical properties. In Decision Support Systems, Elsevier, 47(4):547-553. Dataset retrieved from https://archive.ics.uci.edu/dataset/186/wine+quality on 07/22/2024.
