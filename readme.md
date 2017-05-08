# Classifying Housing Prices

In this project, listings drawn from Zillow.com were classified into a high or low price schemes. 

## Data

The information used in this analysis was scraped from Zillow.com and since a large number of listings existed on that website, I was free to drop null values in order to attain a clean dataset.
The 'type of listing' was the only non-numeric feature included in this project and so I converted it to a series of dummy variables. It may help the reader to understand dummy variables as a series of columns that consists of 1s and 0s. 1, or True, if the unit in question falls under a certain type of listing and 0, or False, if it does not.

## Modeling

After cleaning the data and standardizing it, I experimented with two modeling techniques; Logistic Regression and K Nearest Neighbors. The metric of concern in this analysis was dollars/square foot. The listings that had more valuable units by area when compared to the median listing were considered expensive and the remaining ones were deemed inexpensive (this is the classification that we will aim to predict).

## Conslusions

When experiments were ran in parallel I found K Nearest Neighbors to yield the greatest accuracy when making predictions about the test data that it had never seen before. 84.7% of the time, my model correctly identified a unit as either an expensive or inexpensive unit based on what it learned from the training data. That is a considerable improvement because without a model, random chance would’ve have only guessed correctly about 50% of the time so the existence of this model improves our ability to predict by more than 30%.
