# Logistic Regression and AdaBoost for Classification

## Introduction

In ensemble learning, the combination of decisions from multiple weak learners is employed to solve classification problems. This assignment focuses on the implementation of a Logistic Regression (LR) classifier within the AdaBoost algorithm. For any inquiries regarding this document, please contact Saifur sir.

## Programming Language/Platform

- **Python 3** [Hard requirement]

## Dataset Preprocessing

The performance and efficiency of the implementation should be demonstrated across three different datasets:

1. [Telco Customer Churn](https://www.kaggle.com/blastchar/telco-customer-churn)
2. [Adult](https://archive.ics.uci.edu/ml/datasets/adult)
3. [Credit Card Fraud](https://www.kaggle.com/mlg-ulb/creditcardfraud)

These datasets vary in terms of size, attribute types, data quality, and data descriptions. The core implementation for both LR and AdaBoost models must be adaptable to all three datasets without requiring modification. Dataset-specific preprocessing scripts/modules/functions may be added to standardize data files into matrix format. Additionally, participants may receive another dataset on the submission day, necessitating the creation of a preprocessor.

Suggestions for implementation:

1. **Design and develop original code**: Utilize available resources for guidance but ensure independent implementation.
2. **Handle dataset nuances**: Adapt preprocessing techniques to handle dataset intricacies.
3. **Utilize Python library functions**: Employ Python libraries for common preprocessing tasks.
4. **Reference dataset descriptions**: Thoroughly understand dataset descriptions to ensure accurate preprocessing.
5. **Consider performance**: For the third dataset, efficiency may be prioritized over runtime for demonstration purposes.

Data Splitting:

- Preprocessed datasets should be split into 80% training and 20% testing data if not already divided. Training data exclusively for learning purposes, while testing data solely for performance measurement. Utilize Scikit-learn built-in functions for data splitting.

## Logistic Regression Tweaks for Weak Learning

1. **Attribute Importance Evaluation**: Utilize information gain to assess attribute importance and select a subset of features.
2. **Feature Control**: Incorporate an external parameter to control the number of features.
3. **Early Termination**: Implement early termination of Gradient Descent if training set error becomes < 0.5. Parameterize the function to accept the threshold as input.
4. **Activation Function**: Employ the tanh function instead of the sigmoid function. Adapt gradient calculations and update rules accordingly.

*Published on: 29 Nov 2021*
