# Project - Ames Housing Data and Kaggle Challenge

Welcome to Ames Sousing Data and Kaggle Challenge! It's time to start modeling.


# Overview

This Project look at dataset containing information from the Ames Assessor’s Office used in computing assessed values for individual residential properties sold in Ames, IA from 2006 to 2010. This objective of this project is to accurately predict sales price by minimizing the difference between predicted and actual values. Morever, ensure that performance on a separate test dataset should be comparable to the training dataset to show the model's generailability. And lastly, ensure that the EDA proccess uncover meaningful visual and patterns that provide actionable insight into the data.

The dataset was constructed for the purpose of an end of semester project for an undergraduate regression course. The original data (obtained directly from the Ames Assessor’s Office) is used for tax assessment purposes but lends itself directly to the prediction of home selling prices. The type of information contained in the data is similar to what a typical home buyer would want to know before making a purchase.


---

**Problem Statement**

'Understanding Factors influencing Residential Property Prices through Predictive Modeling and EDA Insights'

--- 

Being cognizant of the factors influencing housing property prices is pertinant for both homebuyers, sellers and investors. I m a data scientist for a real estate investment company and I have been tasked to develop a predictive model that accurately estimates the sale prices of residential properties in Ames, Iowa. The investment firm wants the model to be capable of generalizing well to other data and providing insight into the key features that influence property values. By conducting exploratory data analysis (EDA) and building predictive model, I seek to uncover housing features and trends that will assit key stakeholders on understanding property valuation.

### Provided Data

The dataset that will be choosen for analysis will be **test.csv** and **train.csv.**


**test.csv** "test dataset has all of those columns except for the target ('SalePrice') that I am trying to predict in my regression model.

**train.csv.** train dataset has all of the columns that I will need to generate and refine my models. 



### Data dictionary

[Ames Housing Dataset](https://jse.amstat.org/v19n3/decock/DataDocumentation.txt)

---

#### Brief summary of your analysis

For the baseline model, all models perform relatively well. R² value of 0.8648(lr), 0.8649(lasso), 0.8653(ridge) indicates that the model explains a significant portion of the variance in the target variable, with Ridge Regression having the slightly better R² value among the three. This suggests that Ridge Regression model may be better suited for predicting house price, as the R2 value is an important factor in determining how well a model can accurately predict results. However, for generalizability Lasso and Linear is more suited. 

For the production model I decided to prioritize generalizability and interpretability and selected the Lasso Regression Model. The lasso model the Lasso regression model showed better performance on training and test set when fine-tuned to optimize its predictive performance. When compared to the baseline model, the RMSE on the tuned model is lower which is a positive sign and indicates better generalizarion performance. In summary, given the nature of the problem statement, knowing which features are driving predictions is as important as the accuracy of predictions. The result of this lasso model are more straightforward and interpretable, which is crucial for stakeholders in real estate investment company. 

---

## Conclusions/recommendations

This project looked at understanding factors that influence Residential Property Prices through Predictive Modeling and EDA Insights. Through the Data Science Process, I was able to uncover numerous actionable insights from the dataset that would help investor understand the factors that influence housing property prices. The Ames Housing dataset was a strong way to practice data processing and feature engineering. 

Through this dataset I constructed a model with 96 variables (some of my own creation through interactions), which explains 87% of the variation in sales. While I would consider this model a bit complicated for those who are starting the data science process, it yielded
intuitively appealing coefficients where positive attributes (such as being in certain neighboorhood) added to the value of the home and negative attributes (such as wanting a shed) seem counterintuitive to traditional thinking and subtracted from the value. 

For further analysis, I would recommend fine tuning the features in the datset, using more complex models like decesion trees, random forest, and neural network to get a better indicator of what features influences sales prices. Moreover, identifying property characteristic to predict abnormal sale. The work done by Mattew Perkins and Alvin T. Tan, Ph.D. offers alternative approaches to tackle the Ames housing datset. I would recommend
reading their work to offer more insight to how more knowledge can be gained from this dataset.



---

### Reference

AMES Housing Data — Matthew Perkins. (n.d.). Matthew Perkins. https://www.perkinsml.me/ames-housing

Boyle, T. (2021, December 13). Linear Regression models in Python | towards Data Science. Medium. https://towardsdatascience.com/linear-regression-models-4a3d14b8d368

Tan, A. T., PhD. (2022, March 16). Cracking the Ames Housing Dataset with Linear Regression | Alvin T. Tan | Towards Data Science. Medium. https://towardsdatascience.com/wrangling-through-dataland-modeling-house-prices-in-ames-iowa-75b9b4086c96