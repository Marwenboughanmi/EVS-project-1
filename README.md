# EVS-project-1
## Global Production Data
# Project Overview:
Our group was tasked to compile and analyze data we find useful and prominent in today’s society within the technological field. Using data from the International Energy Agency (IEA), we chose to investigate the development of electric vehicles (EVs) across various countries. To narrow our focus, we programmed the DataFrame to include only the top five and bottom 5 countries with the largest and smallest percentage of electric cars. By graphing the percentage of EVs over time for each country, we conceptualized which countries are leading the transition to electric mobility. 

We also choose to analyze the correlations between electric vehicle deployment and oil gas consumption on a global scale. Using data on all countries' oil consumption, we narrowed it down to the same top five and bottom five countries to compare with EV data. Plotting both DataFrames on the same plot grants us comparability to see if the deployment of EVs in certain countries correlates with oil consumption. 

# Research Questions:

## What are the top five countries that have the greatest percentage of cars that are electric in 2023?

## Is there a correlation between the rise of EV deployment and motor oil gasoline consumption in various countries?

## What does the future percentages of electric cars in each countries look like in a year?

## What is the future prediction of motor oil gasoline consumption in various countries? 

# Data Sources: 

## Running the code: 

### Import the required libraries and dependencies:

!pip install prophet

import pandas as pd

from prophet import Prophet

import datetime as dt

import numpy as npimport matplotlib.pyplot as plt

%matplotlib inline

### Upload csv files for EV data, oil consumption data, and population data
- EV: share-car-stocks-electric.csv
- Oil: energy-consumption-by-source-and-country.csv
- Population: API_SP.POP.TOTL_DS2_en_csv_v2_31753.csv

### Run the Code
- To address our first question regarding which countries have the highest percentage of EVs we isolate the year 2023 for the most recent data, and sort values by percentage.
- To to look for a correlation between oil consumption and the percentage of vehicles that are electric per country:
  - First make sure all data sets have a “Year” index, and merge them together
  - Divide our oil consumption column by our population column to find oil consumption per capita
  - Next create scatter plots of the data to look for correlations 
- To create forecasts for the percentage of EV’s and the amount of oil consumed over the next five years:
  - Format the ev_df and oil_con_df to be compatible with the Prophet model
  - Use Prophet to create five year forecasts for the percentage of EV’s and the amount of oil consumed




