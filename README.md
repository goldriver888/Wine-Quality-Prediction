# Wine Quality Prediction

## Introduction

This project involved the use of machine learning models to predict wine quality levels of red and white vinho verde wine samples, from the north of Portugal. The goal is to model wine quality based on physicochemical tests. The quality levels range from 0 to 10. The models used include Decision Tree, Random Forest, and K-Nearest Neighbors.

## Data Preprocessing

The dataset was downloaded from the [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/dataset/186/wine+quality). It was then collected, cleaned, and transformed for analysis. We ensured high data quality and consistency throughout the process.

Given the imbalance in the classes of the target variable, we used the Synthetic Minority Over-sampling Technique (SMOTE) to oversample the minority class. This technique works by creating synthetic samples from the minor class instead of creating copies, which helps to increase the number of minority class instances and balance the dataset.

## Model Training and Evaluation

The models were trained on a resampled training set and tested on a separate testing set. The performance of each model was evaluated using precision, recall, f1-score, and AUC (Area Under the ROC Curve).

For each model, the quality levels that were predicted most frequently are as follows:

- **Decision Tree Classifier**: The Decision Tree classifier achieved an accuracy of 59%, with an AUC of 0.63. The model most frequently predicted wine quality levels of 5 and 6.

- **Random Forest Classifier**: The Random Forest classifier achieved an accuracy of 64%, with an AUC of 0.68. The model most frequently predicted wine quality levels of 5 and 6.

- **K-Nearest Neighbors Classifier**: The K-Nearest Neighbors classifier achieved an accuracy of 43%, with an AUC of 0.61. The model most frequently predicted wine quality levels of 5 and 6.

The histograms of the original data also show a high frequency of wine quality levels around 5 and 6, suggesting that the models are correctly learning the underlying distribution of the data.

## Conclusion

Among the three models, the Random Forest classifier performed the best in terms of accuracy and AUC. However, there is still room for improvement. Future work could involve tuning the hyperparameters of the models, trying different resampling techniques, or using different features for training the models.

## Recommendations

Based on the analysis, the Random Forest model is recommended for predicting wine quality due to its superior performance. However, it's important to keep in mind the limitations of the analysis and the potential improvements for future work.

## Reference:

Cortez, P., Cerdeira, A., Almeida, F., Matos, T., & Reis, J. (2009). Modeling wine preferences by data mining from physicochemical properties. In Decision Support Systems, Elsevier, 47(4):547-553. Dataset retrieved from https://archive.ics.uci.edu/dataset/186/wine+quality on 07/22/2024.
