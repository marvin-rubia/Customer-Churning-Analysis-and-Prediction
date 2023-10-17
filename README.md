# Customer Churning: Analysis and Prediction for a Telco Company
This repository analyzes customer churning data for a telecommunication company and develops a predictive model that can classify whether a customer will probably churn or not.

## Why analyze customer churn?
Attracting new customers often costs more than retaining customers. In addition, according to [research](https://media.bain.com/Images/BB_Prescription_cutting_costs.pdf) from Bain & Company, Inc., a 5% increase in customer retention can increase profitability by more than 25%. “Return customers tend to buy more from a company over time. As they do, your operating costs to serve them decline. What’s more, return customers refer others to your company.”

## About our dataset
The source .csv file was downloaded via Kaggle from this [link](https://www.kaggle.com/datasets/blastchar/telco-customer-churn). It was a slightly revised version with fewer columns obtained from [IBM's Samples Team](https://community.ibm.com/community/user/businessanalytics/blogs/steven-macko/2019/07/11/telco-customer-churn-1113). It is a dataset for a telecommunication company that offers both phone and internet services. The file has 21 columns.

## Conclusion
__Conclusion from Data Exploration__:

The 17 features that affect customer churning are:

A. Demographic:

1. __SeniorCitizen__ (less likely to churn if senior)
2. __Partner__ (less likely to churn if with a partner)
3. __Dependents__ (less likely to churn if with dependent(s)).
   
B. Offered Services (less likely to churn if subscribed to the following services):

1. __PhoneService__
2. __InternetService__ (less likely if DSL than Fiber Optic)
3. __MultipleLines__
4. __OnlineSecurity__
5. __OnlineBackup__
6. __DeviceProtection__
7. __TechSupport__
8. __StreamingTV__
9. __StreamingMovies__

C. Monetary:

1. __MonthlyCharges__ (churn rate tends to be _high_ around these monetary units: 20, 45, and 80–100)

D. Other Factors:

1. __tenure__ (less likely to churn the longer the customer subscribes to the company)
2. __Contract__ (less likely if 1-year or 2-year contract)
3. __PaperlessBilling__ (less likely if not paperless)
4. __PaymentMethod__ (out of the 4 methods, the electronic check method has a _higher_ churning than the other 3 by a significant margin)

__Conclusion from Predictive Modeling__:

![image](https://github.com/marvin-rubia/Customer-Churning-Analysis-and-Prediction/assets/140475770/b875bd0e-c93b-45ff-beee-e3d12b6e6051)

Out of the five models trained for the telecommunication company's churning dataset, our best model for predicting customer churning is __Gradient Boosting Classifier__ (tuned at `learning_rate=0.1`, the rest of the parameters are default). Its ROC-AUC score is 0.843, its weighted f1-score is 0.780, and its accuracy is 0.79.

## How to see my work?
You can check [my Notebook](https://github.com/marvin-rubia/Customer-Churning-Analysis-and-Prediction/blob/main/Customer_Churning_Analysis_and_Prediction.ipynb) in this repository. Also, the source .csv file is uploaded here.

## I wrote a blog about this
You can also check my article: [Customer Churning: Analysis and Prediction for a Telco Company](https://marvinrubia.medium.com/customer-churning-analysis-and-prediction-for-a-telco-company-9c6bbafa34b3). I wrote it for anyone who has an interest in data analysis and machine learning. 
