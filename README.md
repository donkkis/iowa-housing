# iowa-housing

Multivariate regression analysis of housing prices (data source: https://www.kaggle.com/c/house-prices-advanced-regression-techniques). A notebook for educational/research purposes - everything is very much untested and strictly non-productional!

Main features of the notebook:

* Tech: pandas, numpy, sklearn
* The data has 79 predictor variables incl. categorical and numeric variables
* We employ exploratory analysis and by-hand feature engineering to reduce the predictors down to 55 variables
* Categorical variables are one-hot encoded
* Fitting a linear model to the data, we obtain a MAE score of ~20k in the training set, with the predicted variable ranging between 34900 and 755000

Things to try and improve the result:

 * Introduce more variables - rather arbitrarily, we stripped some off in the very beginning, while in retrospect this might not have been "justifiable"
 * Introduce some form of regularisation: Contrary to "gut feeling" for a linear model, lower MAE in the training set actually suggests we are overfitting our data and
 * Try a more complex model, i.e. polynomial features
 * Introduce a different regression algorithm, e.g. a neural network / deep neural net
