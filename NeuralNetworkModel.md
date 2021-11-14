Introduction
A non-profit foundation, Alphabet Soup, analyzes an algorithm to predict whether or not applicants for funding will be successful. This algorithm utilized machine learning and neural networks to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.
Approach and Results
From Alphabet Soup�s business team, more than 34,000 organizations were provided in CSV format of organizations that received funding from Alphabet Soup over the years. Within this dataset, there are several columns that capture metadata about each organization, such as the following:
1. EIN � Identification columns
2. NAME�Identification columns
3. APPLICATION_TYPE�Alphabet Soup application type
4. AFFILIATION�Affiliated sector of industry
5. CLASSIFICATION�Government organization classification
6. USE_CASE�Use case for funding
7. ORGANIZATION�Organization type
8. STATUS�Active status
9. INCOME_AMT�Income classification
10. SPECIAL_CONSIDERATIONS�Special consideration for application
11. ASK_AMT�Funding amount requested
12. IS_SUCCESSFUL�Was the money used effectively
Pandas and the Scikit-Learn�s StandardScaler() is used to preprocess the dataset in order to compile, train, and evaluate the neural network model.  Of the 12 columns listed above, the identification columns (EIN and Name) were deemed to not be useful for the measurement.  
TensorFlow is used for machine learning and artificial intelligence to focus on training and inference of deep neural networks.  Using TensorFlow, a neural network, or deep learning model, was designed to create a binary classification model to assist in predicting if an Alphabet Soup�funded organization will be successful based on the features in the dataset. This dataset has been compiled, trained, and evaluated to calculate binary classification model loss and accuracy.
1. Number of unique values for each column
APPLICATION_TYPE            17
AFFILIATION                  6
CLASSIFICATION              71
USE_CASE                     5
ORGANIZATION                 4
STATUS                       2
INCOME_AMT                   9
SPECIAL_CONSIDERATIONS       2
ASK_AMT                   8747
IS_SUCCESSFUL                2
dtype: int64

�APPLICATION TYPE� and 'CLASSIFICATION� variables are considered targets for the model.


Conclusion
Seeing the classification project, when ran a several times, did not result in 75% accuracy, selecting the best classification is key.  Classification projects include Logistic Regression, K-Nearest Neighbors (KNN), SVM, Kernel SVM, Naive Bayes, Decision Tree classification, XGBoost and RandomForest classification to name a few.
Another key element is to make sure your data is accurate and usable.  Invalid data can skew the prediction results.  Datas or alpha variables in the income field may distort the prediction accuracy.
