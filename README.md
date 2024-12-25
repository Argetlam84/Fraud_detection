# Fraud Detection



This dataset can be accessed <a href="https://huggingface.co/datasets/Nooha/cc_fraud_detection_dataset">Here</a>

This project was developed collaboratively with <a href="https://github.com/GulsahKLC">Gülşah Kılıç</a>


# Machine Learning Section
Encoded features were created, and two machine learning models—logistic regression and LightGBM (LGBM)—were developed. The following observations were made based on these models:

# Logistic Regression
Logistic regression was found to be ineffective in classifying the imbalanced dataset. Attempts were made to improve the results by applying cross-validation, resulting in an F1 score of 0.499.

# LGBM
The initial performance of the LGBM model was observed to be worse than that of logistic regression, with an F1 score of 0.12. After applying cross-validation, the F1 score was improved to 0.544.

These outcomes were considered to be the worst results encountered in any project. Consequently, research was conducted, and the Synthetic Minority Oversampling Technique (SMOTE) was applied. After this adjustment, the following metrics were achieved with the LGBM model:

- Accuracy: 0.996
- Precision: 0.299
- Recall: 0.606
- F1: 0.400

# Ensemble Modeling
Further efforts were made to enhance the results, and an ensemble approach was implemented successfully. A deep learning model was integrated with the LGBM model, yielding the best results for the project. The metrics achieved were as follows:

- Accuracy: 0.9983
- Precision: 0.9978
- Recall: 0.9989
- F1: 0.9983
