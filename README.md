# ML1 

## Introduction 

A dataset containing information about the height(inches) and weight(pounds) of 200 sample observations from a dataset of 25,000 observations  has been taken. The data is has observations of only 18 year old individuals.

Even though height and weight are mostly dependent on mostly the genetic makeup of the individual surveyed, several other factors like environment, health and lifestyle also influence them. 

These data were simulated in 1993 by a Growth Survey of 25,000 children from birth to 18 years of age recruited from Maternal and Child Health Centres (MCHC) and schools and were used to develop Hong Kong's current growth charts for weight, height, weight-for-age, weight-for-height and body mass index (BMI). See also the Major League Baseball Players Height and Weight dataset.


## Aim

- To model the given dataset 
- To predict the height of an individual for a given weight 

## About the Data

From the given dataset, we can see that there are 2 columns and 200 rows. After checking for duplicates, we observe that there are no duplicates and we retain the dataset as it is. 

There are only two variables and both of them are numeric, thus we can directly jump to analysing their nature.

Now, analysing the continuous variables, we have : 

Now, observing the structure of the data:

Mean and Median:
We see that the mean and median are almost equal, which goes on to show that the dataset has a normal distribution

Inter-Quartile Range and Outliers
Thus Outliers are any values that lie below  Q1 – 1.5 ×IQR or above Q3 + 1.5×IQR. 
We see that the number of outliers are negligible.

Skewness:
We can see that both the variables Height and Weight are fairly skewed.

Variance and Standard Deviation 
We see that the standard deviation of Height is negligible whereas that of weight is moderate. 
Thus they tend toward the central value

Kurtosis:
We see that the kurtosis is close to zero in both the cases

Min-Max and Left3Std and Right3Std
Left3Std means 3 standard deviations below the mean and right3std refers to 3 standard deviations above the mean 
On comparing these values with that of the min-max values of the dataset, we can see that they almost coincide.

## Modelling the Given Data
The data has been divided into a training and testing set on the ratio (80:20) and has been used for modelling.  A Simple Linear Regression Model has been trained on the given dataset. This model is now used to predict the values of the test set.

**The Linear Regression equation is given by: 

Weight = -109.16128390419823 + (Height)*3.47681435 ** 


## Checking Accuracy of the Model 

There are three primary metrics used to evaluate linear models. These are: 
Mean absolute error (MAE), Mean squared error (MSE), or Root mean squared error (RMSE).
MAE: The easiest to understand. Represents average error
MSE: Similar to MAE but noise is exaggerated and larger errors are “punished”. It is harder to interpret than MAE as it’s not in base units, however, it is generally more popular.
RMSE: Most popular metric, similar to MSE, however, the result is square rooted to make it more interpretable as it’s in base units. It is recommended that RMSE be used as the primary metric to interpret your model.





