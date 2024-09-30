# EVS-project-1
## Global Production Data
# Project Overview:
Our group was tasked to compile and analyze data we find useful and prominent in today’s society within the technological field. Using data from the International Energy Agency (IEA), we chose to investigate the development of electric vehicles (EVs) across various countries. To narrow our focus, we programmed the DataFrame to include only the top five countries with the largest percentage of electric cars. By graphing the percentage of EVs over time for each country, we were able to conceptualize which countries are leading the transition to electric mobility. 

We also choose to analyze the correlations between electric vehicle deployment and motor oil gas consumption. Norway was found to have the country with the highest percentage of electric vehicles, 

# Research Questions:

##What are the top five countries that have the greatest percentage of cars that are electric in 2023?

##Is there a correlation between the rise of EV deployment and motor oil gasoline consumption in various countries?

##What does the future percentages of electric cars in each countries look like in a year?

##What is the future prediction of motor oil gasoline consumption in various countries? 

# Data Sources: 

## Running the code: 
Import the required libraries and dependencies:
import pandas as pd
from prophet import Prophet
import datetime as dt
import numpy as npimport matplotlib.pyplot as plt
%matplotlib inline

Import data Evolution of motor oil consumption by product in United States CSV files 

https://origin.iea.org/countries/united-states/oil

Data frame groupby country and year ,once we run it shows you the different entity between the year 2010 and 2023


