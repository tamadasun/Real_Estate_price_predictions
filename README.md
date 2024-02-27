# Project 2 - Ames Housing Data and Kaggle Challenge


**Primary Objectives:**

1. Creating and iteratively refining a regression model
1. Using [Kaggle](https://www.kaggle.com/) to practice the modeling process.
1. Providing business insights through reporting and presentation.

You are tasked with creating a regression model based on the Ames Housing Dataset. This model will predict the price of a house at sale.

The Ames Housing Dataset is an exceptionally detailed and robust dataset with over 70 columns of different features relating to houses.

Secondly, we are hosting a competition on Kaggle to give you the opportunity to practice the following skills:

- Refining models over time
- Use of train-test split, cross-validation, and data with unknown values for the target to simulate the modeling process
- The use of Kaggle as a place to practice data science

Submitt a technical report and a presentation. **You may find that the best model for Kaggle is not the best model to address your data science problem.**

## Set-up

Before you begin working on this project, please do the following:

1. Sign up for an account on [Kaggle](https://www.kaggle.com/)
2. **IMPORTANT**: Click the link [DSI-1113 Ames Regression Challenge](https://www.kaggle.com/t/177bc8cfe89b48d59ee4360ed9b56680) to **join** the competition (otherwise you will not be able to make submissions!)
3. Review the material on the [DSI-1113 Ames Regression Challenge](https://www.kaggle.com/competitions/1113-ames-competition)
4. Review the [data description](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt).

## The Modeling Process

1. The train dataset has all of the columns that you will need to generate and refine your models. The test dataset has all of those columns except for the target that you are trying to predict in your regression model.
2. Generate your regression model using the training data. We expect that within this process, you'll be making use of:
    - train-test split
    - cross-validation / grid searching for hyperparameters
    - strong exploratory data analysis to question correlation and relationship across predictive variables
    - code that reproducibly and consistently applies feature transformation (such as the preprocessing library)
3. Predict the values for your target column in the test dataset and submit your predictions to Kaggle to see how your model does against unknown data.
    - **Note**: Kaggle expects to see your submissions in a specific format. Check the challenge's page to make sure you are formatting your CSVs correctly!
    - **You are limited to models you've learned in class**. In other words, you cannot use XGBoost, Neural Networks or any other advanced model for this project.
4. Evaluate your models!
    - consider your evaluation metrics
    - consider your baseline score
    - how can your model be used for inference?
    - why do you believe your model will generalize to new data?

## Submission

Materials must be submitted by **9 AM Pacific, Friday, December 15**.

The last day for the Kaggle competition will be **11:59 PM Pacific, Thursday, December 14**.

Your technical report will be hosted on Github Enterprise. Make sure it includes:

- A README.md (that isn't this file)
- Jupyter notebook(s) with your analysis and models (renamed to describe your project)
- At least one successful prediction submission on [DSI-1113 Regression Challenge](https://www.kaggle.com/competitions/1113-ames-competition) --  you should see your name in the "[Leaderboard](https://www.kaggle.com/competitions/1113-ames-competition/leaderboard)" tab.
- Data files
- Presentation slides
- Any other necessary files (images, etc.)

**Check with your instructors for how they would like you to submit your repo.**


---

## Rubric

Your local manager will evaluate your project (for the most part) using the following criteria.  You should make sure that you consider and/or follow most if not all of the considerations/recommendations outlined below **while** working through your project.


### The Data Science Process

**Problem Statement**

'Understanding Factors in Residential Property Prices through Predictive Modeling and EDA Insights'

Being cognizant of the factors influencing housing property prices is pertinant for both homebuyers, sellers and investors. I m a data scientist for a real estate investment company and I have been tasked to develop a predictive model that accurately estimates the sale prices of residential properties in Ames, Iowa. The investment firm wants the model to be capable of generalizing well to other data and providing insight into the key features that influence property values. By conducting exploratory data analysis (EDA) and building predictive model, I seek to uncover housing features and trends that will assit key stakeholders on understanding property valuation.

Success will be evaluated through accurately predicting sales price by minimizing the difference between predicted and actual values. Secondly, Performance on a separate test dataset should be comparable to the training dataset to show the model's generailability. Lastly, the EDA proccess should uncover meaningful visual and patterns that provide actionable insight into the data.


### REMEMBER:

This is a learning environment and you are encouraged to try new things, even if they don't work out as well as you planned! **Learn from your failures and you'll be prepared to succeed**.
