# CS105-project

## Introduction
Los Angeles is known for its poor air quality due to high levels of air pollution. Aerosols are an important component of air pollution and can have negative effects on human health. By building a model to predict aerosol concentrations, it can help better understand the relationship and factors between weather conditions and high levels of air pollution in any region. Our objective was to analyze the relationship between weather conditions and atmospheric aerosol concentrations in the Los Angeles, California region.

## Data Sources
We used three different data sets and put them together to create our final dataset. The first dataset consisted of weather data with 45 features from 2000 to 2022. Out of the 45 features, we selected the following: TMIN (min. temperature), TMAX (max. temperature), PRCP (precipitation), and AWND (average daily wind speed). The second dataset contained nitrous oxide data (NOx/pollution) and the third dataset had particulate matter 2.5mm (PM2.5). All three were combined to create our final dataset.

## Analysis
We used K-NN regression to predict NOx and PM2.5. Before starting, the features were standardized with the exception of the target data that we planned to predict. To test our regression model, we used leave-one-out cross-validation. Our value of k was calculated using the square root of the size of the data. When used to predict NOx, our regression model performed well and was able to predict values with low error.

## Results
For the results of our analysis, we can conclude that K-NN regression was great for predicting NOx using maximum and minimum temperature, average precipitation, and average wind speeds. With the output values of mean-squared error from running K-NN regression, predicting NOx achieved a close to 0 value with similar predicted versus actual values. Our model had .98 accuracy and .002 MSE for predicting NOx levels. The K-NN classifier was successful in classifying PM2.5 and NOx measurements into their actual corresponding AQI danger categories. TMAX and TMIN have a strong positive correlation as they are both temperate-related and measure the same values. AWND has a weak positive correlation with TMIN and PRCP. PM2.5 and Avg_NOx have a weak positive correlation. Avg_NOx has a moderate negative correlation with TMIN and AWND.
