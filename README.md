# Diamonds
This is a regression model built to predict a diamond's price based on different characteristics of a diamond.  It is designed to walk through the process of predicting an outcome using a training and test set of data. It is in Jupyter Notebook format.
You can also view the notebook in a browser by clicking on the binder icon below. The link will serve a docker image of the project, so no Jupyter needed.


[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/johnklee54/diamonds/HEAD?labpath=John+Lee+Final+project+notebook-diamonds.ipynb)

The nteobook starts with simple linear regression model. The model will try to use a single indepdent variable (in this case the carat size) to predict a dependent variable (price of the diamond) as this seems to make sense, the larger the carat size the more expensive it should be. 

Using the data provided by Kaggle, the data is a single comma-seprated file (csv) with the following characteristics:

- A data frame with 53940 rows and 10 variables:
- price: price in US dollars (\$326--\$18,823)
- carat: weight of the diamond (0.2--5.01)
- cut: quality of the cut (Fair, Good, Very Good, Premium, Ideal)
- color: diamond colour, from J (worst) to D (best)
- clarity: a measurement of how clear the diamond is (I1 (worst), SI2, SI1, VS2, VS1, VVS2, VVS1, IF (best))
- x: length in mm (0--10.74)
- y: width in mm (0--58.9)
- z: depth in mm (0--31.8)
- depth: total depth percentage = z / mean(x, y) = 2 * z / (x + y) (43--79)
- table: width of top of diamond relative to widest point (43--95)

This project will also use multiple Regression since the initial simple regression will have too many dependent variables (prices) which do not seem to follow the logic from above. In other words, there are more factors involved when pricing a diamond than just the carat size.
We will use R2 and MAE to assess the accuracy of the model. An R2 score of above .9 indicates this model is fairly accurate. Anything below .9 and we are looking into further analysis. For MAE, the lower the MAE is , the more accurate out model is deemed.  
