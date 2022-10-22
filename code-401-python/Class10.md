# Linear Regressions

- **linear regression** is a popular technique and you might as well seen the mathematical equation of linear regression.  You can do linear regression using numpy, scipy, stats model and sckit learn.
- **Linear regression** is a basic and commonly used type of predictive analysis


## Scikit-learn
**Scikit-learn** is a powerful Python module for machine learning, it contains function for regression, classification, clustering, model selection and dimensionality reduction

**run Linear regression --> from `sklearn.linear_model import LinearRegression`**

**Important functions to keep in mind while fitting a linear regression model are:**
- lm.fit() -> fits a linear model
- lm.predict() -> Predict Y using the linear model with estimated coefficients
- lm.score() -> Returns the coefficient of determination (R^2). A measure of how well observed outcomes are replicated by the model, as the proportion of total variation of outcomes explained by the model.


## What is Overfitting/Underfitting a Model?

### Overfitting
**Overfitting** means that model we trained has trained “too well” and is now, well, fit too closely to the training dataset.

### Underfitting
In contrast to **overfitting**, when a model is underfitted, it means that the model does not fit the training data and therefore misses the trends in the data. It also means the model cannot be generalized to new data

## Train/Test Split
**Train set:** The training dataset is a set of data that was utilized to fit the model. The dataset on which the model is trained. This data is seen and learned by the model.

**Test set:** The test dataset is a subset of the training dataset that is utilized to give an accurate evaluation of a final model fit.