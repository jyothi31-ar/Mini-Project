# EXPLORING PUBLIC OPINION ON US AIRLINES VIA TWITTER
**TABLE OF CONTENTS**
1. DATA UNDERSTANDING
2. MODELLING
3. BEST PERFORMING MODEL
4. CONCLUSION


**DATA UNDERSTANDING**



The dataset used in this project is provided from Kaggle and originally collected by Crowdflower’s Data for Everyone library.
This Twitter data was scraped on February 2015. It contains tweets on six major United States (US) airlines: United, Us Airways, American, Soutwest, Delta and Virgin America.
Dataset has 14,640 entries and 15 columns.
We have three different target categories as positive, neutral or negative depend on tweet.


**MODELLING**

The sentiment column served as the target, and tweet column as the predictor variable in our modeling.
Class imbalance was an issue found during modeling.
Logistic Regression, Naive Bayes, Support Vector Classifier were tested as well as LSTM network
Although most of models had overfitting issues, Naive Bayes showed slight improvement on overfitting with the highest F1 score of 91%.

**BEST PERFORMING MODEL**

Throughout the project, our goal was reducing False Negatives and False Positives
False Positive: Model predicts negative tweet but it's actually positive, leading to wrong customer service response and wasting company time/money.
False Negative: Model predicts positive tweet but it's actually negative, leading to lack of proper customer service and potential loss of customer.

**CONCLUSION**

Best accuracy and F1 score were achieved through parameter tuning with SUPPORT VECTOR MACHINE.
