# Customer Churning: Analysis and Prediction
This repository analyzes customer churning data for a Telco company and develops a predictive model that can classify if a customer will probably churn or not.

## Why analyze customer churn?
Attracting new customers often costs more than retaining customers. In addition, according to [research](https://media.bain.com/Images/BB_Prescription_cutting_costs.pdf) from Bain & Company, Inc., a 5% increase in customer retention can increase profitability by more than 25%. “Return customers tend to buy more from a company over time. As they do, your operating costs to serve them decline. What’s more, return customers refer others to your company.”

## About our dataset
The source .csv file was downloaded via Kaggle from this [link](https://www.kaggle.com/datasets/blastchar/telco-customer-churn). It was a slightly revised version with fewer columns obtained from [IBM's Samples Team](https://community.ibm.com/community/user/businessanalytics/blogs/steven-macko/2019/07/11/telco-customer-churn-1113). It is a dataset for a telecommunication company that offers both phone and internet services. The file has 21 columns.

## Conclusion

![image](https://github.com/marvin-rubia/Customer-Churning-Analysis-and-Prediction/assets/140475770/3afd524b-8376-47fb-b1c2-419668d4b013)

Out of the five models trained for the telecommunication company’s churning dataset, our best model for predicting customer churning is the Gradient Boosting Classifier (learning_rate tuned at 0.1, the rest of the parameters are default). Its ROC-AUC score is 0.842 and its weighted f1-score is 0.780.

## How to see my work?
You can check the .ipynb file in this repository. Also, the source .csv file is uploaded here.

## I wrote a blog about this
You can also check my article: [Customer Churning: Analysis and Prediction for a Telco Company](https://marvinrubia.medium.com/customer-churning-analysis-and-prediction-for-a-telco-company-9c6bbafa34b3). I wrote it for anyone who has an interest in data analysis and machine learning. 
