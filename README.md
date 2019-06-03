# Predicting the sign of Dow Jones returns with daily news
News are important in predicting stock returns. Good news about a company are often followed with positive returns whereas bad news are followed by negative returns. Therefore, correctly incorporating the news information in trading strategies is key for the strategies to be profitable. Numerous papers have been proposed to handle this task:
* "Trading Strategies to Exploit Blog and News Sentiment" (Zhang, Skiena 2010)
* "The Predictive Power of Financial Blogs" (Frisbee 2010)
* "An analysis of verbs in financial news articles and their impact on stock price" (Schumaker 2010)


In this study, the problem of stock return prediction will simplified into a classification task. The goal will be to predict whether the Dow Jones Industrial Average a given day is positive or negative given the headline news the given day. 

Datasets and Inputs

For this study, I will use the data from `Sun, J. (2016, August). Daily News for Stock Market Prediction, Version 1. https://www.kaggle.com/aaron7sun/stocknews.`
I will use the Combined_News_DJIA.csv dataset which contains:
* News data: the top 25 historical news headlines from Reddit WorldNews Channel from 2008-08-08 to 2016-07-01. 
* Dow Jones Industrial Average (DJIA) returns as labels: the label is 1 is the return that day is nonnegative and 0 when the return is negative. 

Evaluation Metrics

For task evaluation, I will use data from 2008-08-08 to 2014-12-31 as Training Set and the Test Set will be the following years data: from 2015-01-02 to 2016-07-01.
The classes in the test set are well balanced, therefore we will not consider the AUROC metric and consider simply the Accuracy metric.
