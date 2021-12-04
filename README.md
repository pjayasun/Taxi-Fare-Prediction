# Taxi-Fare-prediction

The data contains only the pickup date & time, the latitude & longitude (GPS coordinates) of the pickup and dropoff locations, and the number of passengers.
I used haversine formula calculates the distance on a sphere between two sets of GPS coordinates. I performed feature engineering on the timestamp and derived useful statistics.


## Categorify
I converted categorical values to numerical codes. A dataset containing months of the year will be assigned 12 codes, one for each month. These will usually be the integers 0 to 11.

## Tabular Model
The goal is to define a model based on the number of continuous columns plus the number of categorical columns and their embeddings and emb_szs respectively. The output would either be a regression (a single float value), or a classification (a group of bins and their softmax values).

* continuous vs. categorical values
* embeddings
* batch normalization
* dropout layers

## RMSE: 3.62
