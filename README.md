# Corporate-Bankruptcy-Prediction

**Predict the bankruptcies of certain companies listed on Taiwan Stock Exchange using data collected from the Taiwan Economic Journal for the years 1999 to 2009.
Tags: Data Science, Data Mining, Machine Learning, Data Analysis**

**Co-created by Harsh Mudgil, Harshal Pawar, Saubhagya Verma and Tawheed Yousuf**

**Summary:**
![image](https://user-images.githubusercontent.com/52705077/132134910-a7696018-f3e5-496c-b806-452c3790bcfc.png)

Predicting the financial health of companies and firms has become one of the key interests for their owners, creditors and all the stakeholders alike, especially now when huge amounts of financial data can be stored and analysed on computers.

The purpose of such a predictive model which tries to foreseee the bankruptcy is to combine various econometric parameters that can effectively guage the financial state of a company and enable the management to take pre-emptive measures that can potentially help to avoid any financial distress to the company.

In this project we present our analysis of the data at hand as we go on selecting various subsets of the huge feature space available to us. We try to compile and compare each and every result as we step from a niave modelling to a more nuanced and standard one. We have employed some of the most widely used classification algorithms for this project namely:

**-Isolation Forest for anamoly detection**

**-Guassian Naiye Bayes**

**-Logistic Regression**

**-Random Forest**

**-Balanced Bagging**

**-SMOOTEEN based XGB**

**-Easy Ensemble Technique**

We began our analysis by visualizing the sparsity of the two target classes (bankrupt and non-bankrupt) in our dataset. Once we were assured of the huge class imbalance in the data we were going to work on, we began to speculate that the prediction could very well be an anamoly detection problem.

We used box plots to visualize how each feature was distributed over each of the two target classes. This gave us a clear idea as to which variable was contributing more to the bankruptcy.

As we delved deep into the dataset it become increasingly clear that the classes had a rich overlap and hence could barely be modelled into an anamoly detection.

Towards the begining, our approach mainly included reducing the dimensionality of the dataset and getting an ideal number of features which could be modelled with ease and effeciency. We employed some of the most commonly used feature engineering techniques like; Threshold Variance, Information Gain, Random Forest, Lasso and a few others to subset our feature space and remove the ominous curse of dimensionality.

Finally we started the machine learning part on the choosen feature subsets, did cross validation for each of the models' hyperparameters and recorded the performance in each case into a compact dataframe. The evaluation metrics we chose for our project include roc_auc score, precision, recall, f1-score.
