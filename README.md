# housing-price-model-selection
Comparison of OLS, Ridge, and Cubic Spline Regression for housing price prediction

## Objective:
Assess differences in regression performance and analyze the bias-variance tradeoff using K-fold CV and test RMSE

## Dataset:
- 545 residential housing observations
- Variables: area, bedrooms, bathrooms, stories, parkings and 7 more binary/categorical features

## Methods:
- Train-test split
- 5-fold CV for Ridge (selecting lambda) and Cubic Spline Regression (selecting number of knots)
- Using the best hyperparameter to finalize the model and compute test RMSE
- Comparing test RMSE between models

## Final Results:
- Ridge Regression has the best performance (lowest test RMSE across all models)
- Moderate regularization reduce variance and improve generalization in prediction

## Tools:
- Python
- pandas
- scikit-learn
- GridSearchCV & Pipeline
- ColumnTransformer
