# Bike Sharing Assignment (BoomBikes)

## **Problem Statement**

A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

A US bike-sharing provider **BoomBikes** has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

- Which variables are significant in predicting the demand for shared bikes.
- How well those variables describe the bike demands <br>

Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors.

**Business Goal**:

You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.

## Table of Contents

- [General Info](#general-information)
- [Technologies Used](#technologies-used)
- [Conclusions](#conclusions)
- [Acknowledgements](#acknowledgements)


## General Information

**Issues to Address:**

1. **Revenue Decline:** BoomBikes faces substantial revenue declines due to the ongoing pandemic, necessitating a strategic solution.
2. **Market Sustainability:** The company struggles to sustain itself in the current market scenario, demanding a mindful business plan.
3. **Post-Lockdown Strategy:** BoomBikes aims to accelerate revenue post-lockdown, requiring an understanding of post-quarantine bike demand.

**Objectives:**
The objectives include predicting significant variables influencing American market shared bike demand, determining the crucial predictors, developing a model to understand demand variations, facilitating adaptive business strategies, and exploring demand dynamics for effective decision-making. This case study aims to achieve this goal by building a multivariate linear regression model using the provided [dataset](./day.csv).

The primary objective is to identify the key variables that significantly influence the prediction of shared bike demand and assess how effectively these variables describe the patterns in bike demands.

## Technologies Used

- [Python](https://www.python.org/) - version 3.12.4
- [Matplotlib](https://matplotlib.org/) - version 3.8.4
- [Numpy](https://numpy.org/) - version 1.26.4
- [Pandas](https://pandas.pydata.org/) - version 2.2.2
- [Seaborn](https://seaborn.pydata.org/) - version 0.13.2
- [Statsmodels](https://www.statsmodels.org/stable/index.html) - version 0.14.2
- [Scikit-Learn](https://scikit-learn.org/stable/) - version 1.4.2

## Conclusions

- The equation of the best fit line is given by:
  - **_cnt_** =  0.1635 + 0.2334 x **_year_** - 0.1036 x **_holiday_** +0.4914 x **_temp_** - 0.1572 x **_windspeed_** + 0.0490 x **_aug_** - 0.0430 x **_jan_** + 0.1110 x **_sep_** - 0.0486 x **_sun_** - 0.2888 x **_Light_snowrain_** - 0.0821 x **_Misty_** + 0.0930 x **_summer_** + 0.1272 x **_winter_**
- The close alignment of R2 and adjusted R2 values between the training and test sets (R2: 0.847 vs. 0.7949 and Adjusted R2: 0.843 vs. 0.783) in a linear regression model indicates effective generalisation. This similarity suggests the model avoids overfitting to the training data and is likely to perform consistently on new, unseen data.
- Bike demand is influenced by features such as **year**, **holiday**, **temp**, **windspeed**, **aug**, **jan**, **sep**, **sun**, **Light_snowrain**, **Misty**, **Summer**, **Winter**.
- Three key feature variables, **temp**, **yr**, and **windspeed**, exhibit the highest coefficient values, indicating their significant impact.

## Acknowledgements

- This project was inspired by live session of upGrad Relevance of Linear Regression Models

## Contact

Created by [@UmraoSinghRawat](https://github.com/umraosr)
