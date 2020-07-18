House Prices - Kaggle Project
-----------------------------------------

The objectif of this Project is to predict `House Prices` using advanced regression techniques. Given a lot of features we have to predict the sale prices for each house. For more details about the dataset [here](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data)


Files
-----------------------------------------

* `HousePrices_EDA.ipynb` : Jupyter notebook containing the code used.
* `train.csv` : The training set
* `test.csv` : The test set
* `data_description.txt` : Full description of each feature


Frameworks
-----------------------------------------

* `Pandas` : Data Wrangling / Data Analysis
* `Searbon` & `regressors.plots` : Data Visualization
* `Sklearn i.e Scikit-learn` `regressors.stats` : Machine Learning model / metric

Choosing the right predictors
-----------------------------------------

* I chose the predictors based on `stepwise-regression`, after I removed/added some features to obtain
a good model

* Choosing the best predictors require an in-depth knowledge in the area.

Model - Metrics
------------------------------------------
* Models : 
	* `Multiple linear-regression` : using R-squared, R(adj)-squared and R-predict squared to evaluate our model to find a tradeoff between `precision-bias` respecting `OLS assumption`

	* `Xgboost Regressor` from xgboost : This model is more robust to overfitting and reach better accuracy (`Cf. HousePrices_EDA notebook`) => We opted for this model

	* `GradientBoostRegressor` from sklearn : Robust to overfitting but Xgboost give better results.

	* `RandomForestRegressor` 

	* **Remark** : With more data we can reduce overfitting in Xgboost and GradientBoost `Cf. Learning Curves`

* Metrics : 
	* `rmse` : root mean squared error

Rank / Score
----------------------------------------

* Rank : `1,336/5068 - TOP 30%`
* Score : `0.12810` with `rmse` as an evaluation metric



