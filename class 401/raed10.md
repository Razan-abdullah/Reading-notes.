# Linear Regression in Python

---

## What Is Regression?


Regression searches for relationships among variables. For example, you can observe several employees of some company and try to understand how their salaries depend on their features, such as experience, education level, role, city of employment, and so on.

This is a regression problem where data related to each employee represents one observation. The presumption is that the experience, education, role, and city are the independent features, while the salary depends on them.


---


## When Do You Need Regression?


Typically, you need regression to answer whether and how some phenomenon influences the other or how several variables are related. For example, you can use it to determine if and to what extent experience or gender impacts salaries.

Regression is also useful when you want to forecast a response using a new set of predictors. For example, you could try to predict electricity consumption of a household for the next hour given the outdoor temperature, time of day, and number of residents in that household.


---


## Problem Formulation


When implementing linear regression of some dependent variable ๐ฆ on the set of independent variables ๐ฑ = (๐ฅโ, โฆ, ๐ฅแตฃ), where ๐ is the number of predictors, you assume a linear relationship between ๐ฆ and ๐ฑ: ๐ฆ = ๐ฝโ + ๐ฝโ๐ฅโ + โฏ + ๐ฝแตฃ๐ฅแตฃ + ๐. This equation is the regression equation. ๐ฝโ, ๐ฝโ, โฆ, ๐ฝแตฃ are the regression coefficients, and ๐ is the random error.

Linear regression calculates the estimators of the regression coefficients or simply the predicted weights, denoted with ๐โ, ๐โ, โฆ, ๐แตฃ. These estimators define the estimated regression function ๐(๐ฑ) = ๐โ + ๐โ๐ฅโ + โฏ + ๐แตฃ๐ฅแตฃ. This function should capture the dependencies between the inputs and output sufficiently well.

The estimated or predicted response, ๐(๐ฑแตข), for each observation ๐ = 1, โฆ, ๐, should be as close as possible to the corresponding actual response ๐ฆแตข. The differences ๐ฆแตข - ๐(๐ฑแตข) for all observations ๐ = 1, โฆ, ๐, are called the residuals. Regression is about determining the best predicted weightsโthat is, the weights corresponding to the smallest residuals.

To get the best weights, you usually minimize the sum of squared residuals (SSR) for all observations ๐ = 1, โฆ, ๐: SSR = ฮฃแตข(๐ฆแตข - ๐(๐ฑแตข))ยฒ. This approach is called the method of ordinary least squares.

---


# How to run Linear regression in Python scikit-Learn :


You know that linear regression is a popular technique and you might as well seen the mathematical equation of linear regression. But do you know how to implement a linear regression in Python?? If so donโt read this post because this post is all about implementing linear regression in Python. There are several ways in which you can do that, you can do linear regression using numpy, scipy, stats model and sckit learn. But in this post I am going to use scikit learn to perform linear regression.


![](./Prices.png)