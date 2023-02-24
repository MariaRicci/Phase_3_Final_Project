# Phase_3_Final_Project

## Business Understanding 

This analysis aims to:
- investigate the presence and significance of patterns of the Customer Churn Rate for the SyriaTel telecommunications company.
- build a classifier predict whether a customer will stop doing business with the company.
Stakeholders who could benefit having this information for the company itself, investors and partners.

Customer Churn What is it?
Customer churn or customer attrition is the phenomenon where customers of a business no longer purchase or interact with the business for products or services.
Churn rate or customer attrition rate is the critical metric that quantify mathematically this phenomenon.

Why is it important?
The customer satisfaction keeps the business running and thriving. Generally, the loss of customers is not sudden but the result of a prolonged succession of unsatisfying experiences or the lack of reward for the loyalty shown.
Building a business, and a reputation, is a risky, challenging and strenous investiment from several points of view. Getting new customers is a even more finance consuming enterprise. As the saying goes "prevention is better than cure", the factors impacting the customer satisfaction can be investigated and actionable inputs can be delivered to prevent the loss.
As the matter of fact, the analysis of the customer churn can consolidate the base business while scouting for new expansion opportunities while avoid crisis and catastrophic consequences on the entire business, even in times of economic instability.

How to calculate it?
Churn Rate = Number of customers lost ÷ Total number of clients at the beginning of the interested time period x 100.
I will evaluate different models both parametric and non parametric.

##Data Understanding 

The dataset is small: 3333 entries, 21 columns. Data give information related to the geographical area, customers services comsumption and the tenure of their relationship with the provider. Aside the local calling plan, that has three different charges base on time: day, evening, night, it is possible to identify two other services that can be added: international calling, with a one for all charge, and a voice mail plan, for which it is not possible to deduce the costs if any are presents. Support service data are also available and provide information related to the number of calls made to it. There are no data related for example to the duration of these calls nor their quality. It would have been interesting for a more targeted analysis and the identifications of patterns the inclusions of information specifically related to gender, age, occupation, contractual options, payment options, state population, density, telcom infrastructures, etc.

No information was given about the circumstances and ways the data were harvested. Features are represented by columns labels are self explanatory.

##Data Preparation
No missing variables were detected. Data manipulation included the modification of the data type from obj and int to float, and the conversion to dummy variables. Columns not useful for medeling were dropped. 

##Conclusion
Results and their meaning in the terms proposed by the business problem were interpreted and explained.
