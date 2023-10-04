Name: Dang Thien Nguyen
NetID DXN210021
Assignment 1
CS4372 - Computer Method for Data Scientist

Wine Quality Data Analysis and Prediction

Overview
This project involved analysis of physicochemical properties and quality ratings for 1599 red wines from the Vinho Verde region of Portugal. The goal was to identify factors that influence subjective wine quality ratings and develop models to predict expert ratings from objective chemical measurements.

Data
The dataset was sourced from the UCI Machine Learning Repository. It contains the following attributes for each wine sample:

Fixed acidity
Volatile acidity
Citric acid
Residual sugar
Chlorides
Free sulfur dioxide
Total sulfur dioxide
Density
pH
Sulphates
Alcohol
Quality (score 0-10)
Analysis
Exploratory data analysis was performed using Pandas, Matplotlib, and Seaborn in Python to understand data distributions and relationships. Key findings:

Alcohol and volatile acidity showed the strongest correlations with quality.
Total sulfur dioxide and density also positively correlated with quality.
Multicollinearity existed between some attributes.
Two supervised regression models were developed to predict quality from chemical properties:

SGDRegressor - Optimized via hyperparameters tuning to achieve test RMSE of 0.634
OLS Regression - Linear model achieved test RMSE of 0.669
SGDRegressor slightly outperformed OLS, indicating subtle nonlinear relationships between attributes and quality.

Conclusions
Alcohol, volatile acidity, and total sulfur dioxide were found to be the most influential objective factors correlated with perceived red wine quality. The optimized SGDRegressor achieved the best predictive performance on test data.

References
P. Cortez, A. Cerdeira, F. Almeida, T. Matos and J. Reis. Modeling wine preferences by data mining from physicochemical properties. In Decision Support Systems, Elsevier, 47(4):547-553, 2009.

Contact
Thien Nguyen- dxn210021@utdallas.edu

Let me know if you would like me to expand or modify this README file in any way. The goal is to provide a high-level overview of the key information from the report to introduce the project on GitHub.

To run Wine Quality Data Analysis and Prediction.ipynb:
Import directly into Google Collab to run
If you want to run this file on Jupiter Notebook or VSCode, you may need to install these package to able to run

Python 3.7
NumPy 1.16.4
Pandas 0.24.2
Scikit-learn 0.21.3
Matplotlib 3.1.1
