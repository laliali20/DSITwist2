# DSITwist2

## Forecasting Popularity of Krarken as a Crypto Trading Exchange Meduim

This repo contains code and other resources for a model that forecasts the number of visits for wikipedia articles as well as the goodle trend expected over the next one year.


### About the project 

The goal of the competition was to accurately make a 12 month forecast on the expected number of visits to the firm's wikipidea page as well as the google trends searches.  

The data is based on the Crypto firm Kraken historical searches and visits to it's wikipedia articles. Tweets are also considered for the project. However, due to the complexity in determining a negative tweet from a positive one, this analysis is abandoned. 

From the forecasts, the firm may be able to tell whether it may be able to reach it's reach out goals on publicity which is generally expected to translate into actual demand for crypto buyouts. 

### Contents
* [Overview](#overview)
* [Technologies](#technologies)
* [Setup](#setup)
* [Notebook](#notebook)


### Overview
Daily observations data is initially scraped and then saved into a database. 

The next step is to format it into a monthly time series. This becomes the input into the forecast models. 

The forecast model is picked out based on a holdout sample approach, where the perforrmance of the test set is evaluated on the MAPE accuracy metric. 

The best performing model is applied to give the 12 month prediction, which is the goal of the project.


### Notebook
The code and report for training and forecasting on the google trend and wikipedia page visits is in this [notebook](https://colab.research.google.com/drive/1IzcmZ5Ozk6kvHq42yjGkLYKyMOTC3MzV?usp=sharing)

#### Performance Models Used
The performance ofthe models applied is evluated based on Mean Absolute Percenta Error (MAPE) 
