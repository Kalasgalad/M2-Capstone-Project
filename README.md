# M2 Capstone Project

## Project Overview

This project aims to analyze two datasets containing factors that contribute to overall happiness within a given country. The first goal is to observe the different features in the datasets, and draw some initial relationships that could contribute to the production of a machine learning model. With these relationships illustrated, two machine learning models will be developed and compared such that final predictions will made with the best performing one. <br> This is the link to both datasets used in this project: https://www.kaggle.com/datasets/ajaypalsinghlo/world-happiness-report-2021

Order of operations for this project.

1. Exploratory Data Analysis
2. a) Data Visualization
   b) Initial Comments
3. Feature Engineering and Model Building
4. Model Comparison & Analysis
5. Final Model & Predictions
6. Closing Thoughts


At first glance, a few preliminary relationships can be drawn:
- Higher GDP per capita leads to a higher happiness score.
- Most of the world's population seem to have an average to above average happiness score (rough generalization).
- The top performing countries are mostly all in Europe and belonging to Nordic countries, while the majority of the least performing countries are of African/Arabic origin.

## Models used: Linear Regression and Random Forest Regression

LR: Linearity, scales, assumes relatinship between target variable and features, low overfitting risk.<br>
RF: Captures non-linearity, does not require scaling to perform, more complex modelling.<br>

**Training Model Comparisons:**
Linear Regression - MAE: 0.4211, MSE: 0.2899, R²: 0.7623
Random Forest - MAE: 0.2940, MSE: 0.1509, R²: 0.8763

**Overall we can observe that there are far more blue dots away from the center of the line which is due in large part to the evaluation metrics in the Linear Regression model being lower.<br> Because of this, the Random Forest is likely the better choice as it will produce a prediction with more accuracy**

## Final Model and Prediction (Random Forest)

Input data Life Ladder Score (Happiness Score) : 7.103

Final Prediction
Predicted Happiness Score: 7.18 

### Closing Thoughts

In conclusion, the final chosen model has predicted quite accurately what the life ladder score the second dataframe contained! <br>
The model predicted an outcome of 7.18 Life Ladder Score compared to 7.103 from the actual value from unseen data. <br>
When entering personal inputs, I chose to predict the happiness score for Canada because that's where I live. In these turbulent, sociopolitical times, I want to evaluate if Canadians will still believe that we are an amazing country to grow in. <br>
I've always believed that Canadians aspire to be in the upper echelon of global citizens, so this prediction is personal to me. <br>

Although the dataset that this model is based off of contains subjective data; the predicted happiness score is extremely close to its 2021 evaluation. This leads me to believe that there is a likely chance that Canadians will hold fast to the changes we are faced with this year.
