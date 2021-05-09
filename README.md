# W7-Kaggle_competition

![Imagen_text](https://github.com/Carmen-r/W7-Kaggle_competition/blob/main/images/diamond.jpg)


## Objetive

Predicting diamond prices using Machine Learning models.

## Steps of the proyect:

### Analysis of the variables

#### Target Variable: Price

![Imagen_text](https://github.com/Carmen-r/W7-Kaggle_competition/blob/main/images/Target.jpg)

#### Quantitative variables 

`carat`: weight of the diamond

`x`: length in mm

`y`: width in mm

`z`: depth in mm

`depth`: total depth percentage = z / mean(x, y) = 2 * z / (x + y) (43--79)

`table`: width of top of diamond relative to widest point (43--95)

#### Qualitative variables

`cut`: quality of the cut (Fair, Good, Very Good, Premium, Ideal).

`color`: diamond colour

`clarity`: a measurement of how clear the diamond is

There were no null values, the only thing that was needed was to convert the categorical variables to numerical ones by means of a dictionary.


### Models
` Linear Regression`

`Ridge`

`Lasso` 

`SGDRegressor`

`KNeighborsRegressor`

`GradientBoostingRegressor`

`RandomForest`:  We did the Tune Hiperparameters with `Hyperopt`

`XGBRegressor`: We did the Tune Hiperparameters with `GridSearchCV`

![Imagen_text](https://github.com/Carmen-r/W7-Kaggle_competition/blob/main/images/conclusion.jpg)

### Conclusion

After comparing the models we can affirm that in this case the best option has turned out to be the `XGBRegressor`. For this we have used `GridSearchCV` which has allowed us to choose the best parameters.
