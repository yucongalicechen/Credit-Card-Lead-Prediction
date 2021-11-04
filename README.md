# Credit-Card-Lead-Prediction
Authors (in aphabetical order): Yucong Chen, Haocheng Liao, Kaiqi Peng, Danlei Wang, Wenting Yang

## Introduction
Happy Customer Bank is a mid-sized private bank that operates a variety of banking products, such as
savings accounts, current accounts, investment products, credit products, etc. It also cross sells products to
existing customers through different means of communication. In this case, the bank hopes to cross sell its
credit cards to existing customers.
Our goal of this project is to help Happy Customer Bank to conduct a credit card lead prediction - to identify
customers who have higher intention to recommended credit cards from a qualified group identified by the
bank - through data analysis and models.

For the full project, please see the attached pdf.

## Conclusion
In conclusion, by using and comparing various models and analysis results, we have successfully identified
the logit model as our best model, and come up with a recommended list of potential customers who are
most likely to take credit cards from Happy Customer Bank.
The best model was chosen with some difficulty, as throughout our analysis, a range of possible models
seemed suitable at first sight. For example, the OLS model, the probit model, and the logit model showed
similar results in their summary, their model accuracy, their average marginal effect for each variable, etc. All
estimators were statistically significant in these three models, and the signs of the estimators were consistent.
The logit model showed slightly better model accuracy. To evaluate their performance better, we divided the
data into training data. And logit model still had higher accuracy as well as lower RMSE.
However, this was far from the time when we determined the logit model as our best model. A large range
of tests was provided. For example, RESET test was used to check the model specification, and BP test was
used to detect heteroskedasticity. The logit model passed most of the tests. Furthermore, a multinomial logit
model and an IV model were used to challenge the logit model to see if they were better, but they failed
because other tests have shown that they were either questionable or not well specified.
Although we have identified the logit model as our best model, we still have many shortcomings at present,
such as heteroskedasticity. Though we converted our standard errors into robust standard errors, this did
not help much.
Nevertheless, applying the logit model to our data, lists of recommended customers sorted according to
their level of interest in taking credit cards came out. Based on our result, 3,591 pcustomers are most likely to
take a recommended credit card. Top recommended customers turn out to be mostly males, aged between 40
and 80, self-employed, and are those who tend to choose channel code “X3”, have no active credit product,
have the vintage of about 120 and average account balance between 2 million and 10 million dollars. Most
are active users and live in RG268. These results show the common features of the most recommended
customers and we hope it will help Happy Customer Bank make future decisions about recommending
credit cards and other financial products.

## References
https://www.kaggle.com/sajidhussain3/jobathon-may-2021-credit-card-lead-prediction?select=test.csv
