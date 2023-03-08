# Phase_3_Final_Project

## BUSINESS PROBLEM UNDERSTANDING

This analysis aims to:

investigate the presence and significance of patterns of the Customer Churn Rate for the SyriaTel telecommunications company.

build a classifier predict whether a customer will stop doing business with the company.

Stakeholders who could benefit having this information for the company itself, investors and partners.

I will evaluate different models chosen as appropriate to solve a binary classification problem.

- Naive Gaussian Bayes

- Bernouilli

- Random Forest

- Support Vector Machine

Models fitting will be evaluated by the scores:

- Precision

- Recall

- Accuracy

- F1-score

- AUC and ROC curve

### Customer Churn

What is it?

Customer churn or customer attrition is the phenomenon where customers of a business no longer purchase or interact with the business for products or services.

Churn rate or customer attrition rate is the critical metric that quantify mathematically this phenomenon.

### Why is it important?

The customer satisfaction keeps the business running and thriving. Generally, the loss of customers is not sudden but the result of a prolonged succession of unsatisfying experiences or the lack of reward for the loyalty shown.

Building a business, and a reputation, is a risky, challenging and strenous investiment from several points of view. Getting new customers is a even more finance consuming enterprise. As the saying goes "prevention is better than cure", the factors impacting the customer satisfaction can be investigated and actionable inputs can be delivered to prevent the loss.

As the matter of fact, the analysis of the customer churn can consolidate the base business while scouting for new expansion opportunities while avoid crisis and catastrophic consequences on the entire business, even in times of economic instability.


## EXPLORATORY DATA ANALYSIS

It is a dataset from SyriaTel, provided by Kaggle, and includes 3333 entries spread on 21 columns, whose labels are straightforward.

Data give information related to the geographical area, customers services consumption and the tenure of their relationship with the provider.

Aside the local calling plan, that has three different charges, all based on time: day, evening, night.

It is possible to identify two other services that can be added: international calling, with a one for all charge, and a voice mail plan, for which it is not possible to deduce the costs if any are presents.

Support service data are also available and provide information related to the number of calls made to it.

There are sensitive data as telephone numbers.

There are no data related for example to the duration of these calls nor their quality.

While no missing values are present, plotting shows outliers.

Outliers were kept as the dataset mean after outliers data manipulation is not significantly affected.

Also:

- 17% of the customer sample has dropped out the membership
- 11% of the customers in the sample has an international plan 
- 38% of the customers has a voice mail plan 

## RESULTS DISCUSSION

Accuracy is the metric generally used to evaluate and compare models. It is calculated by the total number of true positives and true numbers are divided by the total number of observations. 

In this case it is possible to state that:

- Naive Gaussian Bayes: 0.87

- Bernouilli: 0.84

- Random Forest: 0.98

- Support Vector Machine: 0.94


Accuracy though, can be misleading and it is advisable to consider the other metrics provided, according to the best suitable business scenario.

Given the values assigned above:

- True Negatives are the customers that don't churn that are correctly identified. 

- False Negatives are the customers incorrectly identified as not intending to churn.
 
- True Positive are the customers that churn.

- False Positive are customers uncorrectly identified as churners.


Which customers are important to this company?

False Negatives and False Positives. Specifically False Negatives. Not only it is more expansive to acquire new customers in stead of the lost ones but also, a wrong evaluation, can mine goals and final balances.




Given that, it is more important to consider precision and recall:


- Precision. Out of all the customers that the model predicted would churn, customers who actually did were:

    - Naive Gaussina Bayes: 57% 
    
    - Bernouilli: 47%
    
    - Random Forest: 100%
    
    - Support Vector Machine: 98%
    
- Recall. Out of all the customers that actually churned, the model only predicted this outcome correctly for these customers:

    - Naive Gaussina Bayes: 55% 
    
    - Bernouilli: 17%
    
    - Random Forest: 88%
    
    - Support Vector Machine: 65%


- F1 Score. This metric indicates how well the model predicts the churning choice. The closer the value is to 1, the better the model performs. Examining the values:

    - Naive Gaussina Bayes: 0.56 
    
    - Bernouilli: 0.25
    
    - Random Forest: 0.93
    
    - Support Vector Machine: 0.78
    

- ROC and AUC. 
ROC summarizes the performance of a binary classification model on the positive class.
AUC function takes both the true outcome from the test set and the predicting set for the positive class.
    
    - Random Forest: models performs almost perfectly discriminating True Positive and False Positive.
    
    - Support Vector Machine: model performs as an unskilled classifier. 

## CONCLUSION

According to the interpretation of these results, it can be stated that the Random Forest is the model that performs best as a classifier for this dataset

### RECOMMENDATIONS

Focus research and improvements in the three catagories analized by the model: focusing on offering a better customer service and more favorable rates for day calls. 


### FURTHER RESEARCH

- Extend application of features selection and other models.

