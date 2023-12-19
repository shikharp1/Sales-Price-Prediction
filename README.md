# Sales-Price-Prediction

![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/d12e737c-1a9c-47b0-9525-3516c2a05a11)
Corporación Favorita is a major grocery retailer with operations in hundreds of supermarkets throughout Ecuador. They carry a variety of products on their shelves. 

A key factor in a company’s retail performance is the ability to properly estimate sales and manage inventories. The key problem is predicting the sales and inventory requirements for each location to avoid overstocking and understocking, allowing the business to offer the greatest customer service while reducing losses and guaranteeing the store’s sustainability.

Data Understanding
The dataset consists of 6 different files:
1.  Train: The training data, comprising time series of features   store_nbr, family, and onpromotion as well as the target sales.
2.  Test: The test data, having the same features as the training data.
3. Transactions: Contains date, store_nbr and transaction made on that specific date.
4. Stores: Store metadata, including city, state, type, and cluster.
5. holidays events: Holidays and Events, with metadata.
6. oil: Daily oil price which includes values during both the train and test data timeframes. (Ecuador is an oil-dependent country and its economic health is highly vulnerable to shocks in oil prices.)

![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/b76ae93f-bcc4-49d4-99b9-d3e3c72111ba)

Data Preparation
Preparation of Data consist of various Steps such as :

Data Importation
Data Cleaning
Duplicate Values
Data Reduction
![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/6270797c-47b4-4f6c-ab32-852aea6d0fc2)

Exploratory Data Analysis
Univariate Analysis:
![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/032b781d-7274-45c6-86d3-c3e06c57d002)
![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/c12f4d45-3b05-49cd-acd1-32c677b4c30f)
![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/1f9eb3a3-0017-4c6a-957e-0d46f6dfb26f)
![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/da3d50b4-09f1-469b-ab56-c4bea09cb5c0)

Multivariate Data Analysis
![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/1373a1f8-3727-4ff8-ad1b-0578f14ae13d)

![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/7597ccca-9884-4dd7-9c1f-6457b8c4ed4c)

![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/d274d205-c739-468f-ad3d-b0a4d6c5dfd0)

![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/f63d910c-69a3-4480-ad29-b00bf24103fa)

Linear Regression Model:  

Linear regression is a statistical method used to model the relationship between a dependent variable and one or more independent variables. 
In the context of store sales, it predicts future sales based on historical data trends.

![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/0b549083-0684-4835-b518-1ad64a73eceb)

Random Forest Regressor Model:

Random Forest as an ensemble learning method for regression that combines multiple decision trees for more accurate and stable predictions.Strengths:  handling large data sets with higher dimensionality 
Limitations: model complexity and computational intensity


![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/f8784918-612c-40bc-bed5-f36cfc085540)

CatBoost Regressor Model:
CatBoost is a state-of-the-art machine learning algorithm that excels in handling categorical data, making it highly suitable for predicting store sales which often involves diverse data types.
Applications in Sales Forecasting: Practical applications, such as forecasting daily or weekly sales, adjusting for seasonal trends, and promotions impact analysis.

![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/7636ece1-1ada-4580-9c23-4bc287c49b3c)

XGBoost Regressor Model:
XGBoost stands for eXtreme Gradient Boosting and is renowned for its efficiency and effectiveness in predictive modeling, especially in scenarios like store sales forecasting where precision and speed are crucial

Can handle different types of sales data, including continuous and categorical variables.

![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/8797dbb1-cfb9-4fdc-ad8d-14f8dd7a592e)

Decision Tree Regressor Model:

A Decision Tree Regressor is a non-parametric supervised learning method used for predicting continuous outcomes, like store sales, by segmenting the data into branches based on decision rules.

Decision trees inherently perform feature selection, choosing the most informative features for splitting.

![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/209c6e50-0ec0-4eb4-9d04-25a355e2f58f)

Comparison of Different Models:

![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/167d5687-625f-45ce-8b00-948e26a75c1c)

Hyperparameter Tuning:

Hyperparameter tuning can improve the RMSLE (Root Mean Squared Logarithmic Error) of a regression model by selecting the hyperparameters that result in the best performance on the validation set

Since Linear Regression did not perform too well, we have decided to use hyperparameter tuning to improve the model. 

![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/52c925d1-3f3c-4a5a-8f3b-e0760428c925)

As can be observed there was no significant improvement in the RMSLE metric even with hyperparameter tuning and feature importance. 

![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/217ede32-3d45-430e-a26b-972ed5d1af02)

Feature Importance:
Feature importance is a technique for understanding the relative importance of features in a model. It involves assigning a score to each feature based on its contribution to the overall performance of the model. The scores can then be used to identify which features are the most important for making accurate predictions and which features may be redundant or even detrimental to the model's performance

![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/01fd83ac-7c95-49a8-80b4-e7e84b14d446)

Model Selection and Evaluation:

![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/4af0969c-7e6a-48b9-81f6-0a339400a783)

Time Series Analysis:

![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/ecf0f321-02eb-4cdf-9f6a-d767a670e565)


Model Deployment:
Deployment of the XGBRegressor Model (After feature importance) : 

![image](https://github.com/shikharp1/Store-Sales-Forecasting/assets/64658989/f2d6557d-259e-4acb-ae8f-e9404996bac9)

Conclusion:

This sales forecasting project, leveraging exploratory data analysis and machine learning models, successfully predicts future sales for Corporation Favorita. Through a combination of regression and time-series models, we achieved an accurate forecasting tool. The evaluation on the test set instills confidence in its potential to guide informed decisions on inventory management and sales strategies.

Key Conclusions and Recommendations for Corporation Favorita:
Understanding Customer Behavior
Product Assortment Optimization
Strategic Promotions and Discounts
Efficient Inventory Management
Data-Driven Decision Making






















