# BT4012

The dataset for the project can be found here: https://www.kaggle.com/datasets/shivamb/real-or-fake-fake-jobposting-prediction 

The alternative models code has EDA, feature engineering.  It is mostly the use of unstructured data to input into a few models such as random forest, SVM, logistic regression and neural networks.

The NLP ensemble method takes advantage of two levels.  The textual columns are cleaned, tokenized, stemmed and lemmatized.  Five BOW matrices and five TF-IDF matrices were obtained from the textual columns.  They were then fed into 10 Multinomial Naive Bayes to generate 10 sets of predictions.  The predictions were then fed into a RFC, SVM and logistic regression model at the second level.  I found that the SVM obtained the best f1 score ~0.84 and ROC-AUC ~0.9.

The ensemble technique used is known as stacking and is extensible to other datasets that have multiple text columns that independently are able to generate predictions.  
