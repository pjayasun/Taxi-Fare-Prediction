# Taxi-Fare-prediction

The data contains only the pickup date & time, the latitude & longitude (GPS coordinates) of the pickup and dropoff locations, and the number of passengers.
I used haversine formula calculates the distance on a sphere between two sets of GPS coordinates. I performed feature engineering on the timestamp and derived useful statistics.

To me, the project looked simple as it was comparable to the Uber fare calculation in day-to-day life, but it was intriguing from the feature perspective. I pondered what the model could learn from the timestamp, latitude, and longitude. So as part of feature engineering, the first thing that came to my mind was distance. I used the haversine formula to calculate the distance between two sets of GPS coordinates and then extracted the hour of the day and other valuable characteristics from the pickup time for surge fee. To further stand out from the crowd, I considered daylight savings time and converted categorical values to numerical codes to make the prediction precisely. The model performed well and exhibited a relatively low RMSE.![image](https://user-images.githubusercontent.com/18529823/146003773-96b47c0b-b311-46b4-81cd-245140d905b1.png)



## Categorify
I converted categorical values to numerical codes. A dataset containing months of the year will be assigned 12 codes, one for each month. These will usually be the integers 0 to 11.

## Tabular Model
The goal is to define a model based on the number of continuous columns plus the number of categorical columns and their embeddings and emb_szs respectively. The output would either be a regression (a single float value), or a classification (a group of bins and their softmax values).

* continuous vs. categorical values
* embeddings
* batch normalization
* dropout layers

## RMSE: 3.62
