# EVS-project-1
## Global Production Data
Authors: Esha Sharma, Jason Clibanoff, Marwen Boughanmi 
# Project Overview:
Our group was tasked to compile and analyze data we find useful and prominent in today’s society within the technological field. Using data from the International Energy Agency (IEA), we chose to investigate the development of electric vehicles (EVs) across various countries. To narrow our focus, we programmed the DataFrame to include only the top five and bottom 5 countries with the largest and smallest percentage of electric cars. By graphing the percentage of EVs over time for each country, we conceptualized which countries are leading the transition to electric mobility.

We also choose to analyze the correlations between electric vehicle deployment and oil gas consumption on a global scale. Using data from all countries' oil consumption from ‘Our World In Data,’ we narrowed it down to the same top five and bottom five countries to compare with % EV data. Plotting both DataFrames on the same scatter plot grants us comparability to see if the deployment of EVs in certain countries correlates with oil consumption per capita.

Another aspect of our project consists of using a Prophet model to forecast EV deployment and oil consumption on a global scale. Furthermore, artificial intelligence has helped us generate predictive insights, enabling informed projections about future oil consumption and EV deployment. 


# Research Questions:

1-Does the rise in EV adoption align with a global drop in oil consumption?

2-How much might global percentages of EVs increase in the next few years?

3-How much might global oil consumption decrease in the next few years?

# Data Sources: 
1-https://ourworldindata.org/grapher/share-car-stocks-electric?tab=map&time=earliest&showSelectionOnlyInTable=1

    a-Shows % of cars that are electric in each country over time

2-https://data.worldbank.org/indicator/SP.POP.TOTL

    a-Global population data over time

3-https://ourworldindata.org/grapher/energy-consumption-by-source-and-country

    a-Oil Consumption over time

## Running the code: 
1-Import the required libraries and dependencies:

a-import pandas as pd
  from prophet import Prophet
  import datetime as dt
  import numpy as np
  import matplotlib.pyplot as plt
  %matplotlib inline

2-Upload csv files for EV data, oil consumption data, and population data

  a-EV: share-car-stocks-electric.csv

  b-Oil: energy-consumption-by-source-and-country.csv
  
  c-Population: API_SP.POP.TOTL_DS2_en_csv_v2_31753.csv

3-To address our first question regarding which countries have the highest percentage of EVs we isolate the year 2023 for the most recent data, and sort values by percentage.

4-Run the code to look for correlation between oil consumption and the percentage of vehicles that are electric per country:

  a-First make sure all data sets have a “Year” index, and merge them together
  
  b-Divide our oil consumption column by our population column to find oil consumption per capita
  
  c-Next create scatter plots of the data to look for correlations 

5-Use Prophet to create forecasts for the percentage of EV’s and the amount of oil consumed over the next five years

# Results:

# Results 1: Correlation between EVs and Oil Consumption

# Task 1: 
Run the code to find the percentage of vehicles that are electric in the top and bottom five countries. First, the code assembles bar graphs that display the top and bottom five countries by the percentage of vehicles that are electric. 

![Top 5 countries by percent of cars that are electric](https://github.com/user-attachments/assets/911925cd-e518-4cda-ab08-7588d07ee801)

![bottom 5 countries by percent of cars that are electric](https://github.com/user-attachments/assets/a2f12172-b191-4576-9e78-51e9b253eff3)

# Task 2:
Then continuing to compile the code, a line graph is produced that shows the top five countries plotted over time. The results demonstrate that Nordic countries are the lead in EV deployment globally. 

![top 5 percentages over time](https://github.com/user-attachments/assets/ff997ff7-4737-412a-aa5b-8a1d275e5061)

# Task 3:
Next the code compiles a global analysis by plotting the percentage of vehicles that are electric vs the oil consumption on the global scale. The following results demonstrates a correlation of -0.0725 between the percentage of EVs and global oil consumption per capita, indicating little to no consistent trend.

![Percentage of Vehicles that are Electric VS Oil Consumption - all countries](https://github.com/user-attachments/assets/8e726436-8dd0-45a7-b194-1a8ec8b86312)

# Task 4:
The code finally graphs the resultant top and bottom five countries of % EVs vs Oil Consumption per capita. The correlation between variables for the top 5 countries excluding Iceland demonstrates there is a gradual decline in oil consumption per capita as there are higher percentages of EVs. The bottom five countries with the lowest percentage of EVs, demonstrates an inconsistent trend that demonstrates the minuscule effect the low percentage of % of EVs have on oil consumption per capita.

![Percentage of Vehicles that are Electric VS Oil Consumption - top 5 countries](https://github.com/user-attachments/assets/33347240-3533-43c3-98c0-2535a4f1c954)

![Percentage of Vehicles that are Electric VS Oil Consumption - bottom 5 countries](https://github.com/user-attachments/assets/79dacf0c-c3d0-4652-838e-0efc9cc62ea5)

# Analysis: 
There is still a long way to go for countries to decrease their oil consumption. Though electric vehicles are growing in the industry, their current adoption rate is not sufficient enough to significantly reduce global oil consumption. Major shifts in nations’ policies, infrastructure, and consumer behavior are required to accelerate the sustainable energy consumption. 


# Results 2: Forecasting the Percentage of EVs Globally

# Task 1: 

we ran the code with a prophet model to get the percentage of EVs globally forecasted for five years.The code showed that the percentage of vehicles that are electric is increasing by 4% in the worst case, 8% in the most likely and 11.3% in the best case for the five year forecast.
This growth could lead to a notable reduction in oil demand.


![5 year forecast for percentage of vehicles that are EVs](https://github.com/user-attachments/assets/a9ce4726-35ef-4084-874c-3a453ec86932)

# Analysis:
The global percentage of electric vehicles is expected to increase significantly over the next few years, driven by advancements in technology, government incentives and falling battery costs. The growth in the percentage of EVs on the road varies by region, but global trends point toward a steep rise in EV adoption.


# Results 3: Forecasting Oil Consumption Globally
# Task 1:

in another code using the prophet model , we tend to forecast the oil consumption globally for the next five years where the average consumption is not showing notable decrease.The result demonstrate how might oil consumption decrease

![Five Year Forecast of Oil Consumption](https://github.com/user-attachments/assets/a41ff8c8-f2af-4dff-a1e5-915427e4e4ea)


# Analysis:
 
 Globally,  oil consumption is not showing a significant decline,compared to the rise for EVs globally for five years forecast. Eventually it is expected to decrease over the next few years, still the exact decline depends on how quickly the world transitions to cleaner energy sources and technologies.








