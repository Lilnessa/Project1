# Project1

Project by Vanessa Dumlao, Shruti Palur Mallampalli, and Noelle Watson

## Overview
The Project 1 Repository consists of data pertaining to gas prices in San Diego. The project explores gas prices in San Diego to see how factors such as zip code, household income, and population density affect these prices. 

The repository contains the Resource folder, the Fig_ouput folder, and two Jupiter Notebook files. 

The Resource folder contains three csv files that hold all of the source data and two csv files that were generated from the two Jupyter Notebook files.

The two Jupyter Notebook files, the gas_price_zip_code.ipynb script, and the charts.ipynb script. The gas_price_zip_code.ipynb takes the source data from two csv files, combines them according to zip code, and outputs the Zip Code All Data.csv file. The script also outputs the extra_clean_gas.csv, which has the cleaned data from the gas-prices-10-04.csv file. The charts.ipynb script takes the outputted csv files, analyzes the data, and produces various charts.

The Fig_output folder contains all of the figures that were generated by charts.ipynb script.

## Data Source and Gathering
The data used in Project 1 comes from Three different sources. The second set of data, which can be found in gas-prices-10-04.csv, was generated by Gas Prices Scaper, an API that collects that day’s current gas prices at every gas station whose prices are listed on Google Maps within the search parameters. The data within gas-prices-10-04.csv comes are the gas prices from October 4, 2023. The area in which data was collected was determined by the zip codes that were available in the Household Income Median.csv file. The Household Income Median.csv file was generated from simplemaps.com for the area of San Diego. The third set of data can be found in the uszips.csv file, which was generated by **I DONT KNOW, PLEASE INPUT BEFORE SUBMISSION**.

## Overview of printed figure
In the charts.ipynb file, the extra_clean_gas.csv file, and the Zip Code Data All.csv file were analyzed, and eight figures were generated in response to _four questions_:

1. How are zip codes and gas prices affected by gas station brands?
2. How does zip code affect differences in gas prices between types?
3. How does the population of a zipcode affect gas prices?
4. How does the median household income of a zipcode affect gas prices?

Looking at question 1, how are zip codes and gas prices affected by gas station brands, two figures were generated: a stacked bar graph of brands by zip code and a bar graph of the average gas price by gas station brands. From the two figures, it can be seen that the number of brands of gas stations in zip codes varies from 1 to 9 and that the average price of gas by brand ranges from $5.70 to $6.50 USD/gallon. Based on the two figures together, it does not seem that zipcodes and gas prices are affected by gas station brands.

Looking at question 2, how does zip code affect differences in gas prices between types, two figures were generated: a stacked line plot of Regular, Midgrade, and Premium gas prices per zip code and a stacked scatterplot of Regular, Midgrade, and Premium gas prices per zip code that were ordered by average income. From the first figure, Gas Prices Per Type vs. Zip Code, each line for the different types of gases is extremely similar to each other, with the gaps ranging from approximately $0.10 to $0.20. The third figure, Gas Price per Type vs Average Income per Zip Code, is the scatterplot of the gas price for each type of gas plotted against the income of each zip code, with a linear regression line plotted for each gas type. The slope for all three types of gas is very small, to the order of negative seven, and all similar to each other. In addition, the r-squared values for all three lines are all less than 0.04, indicating that the differences in price between the types of gas are not affected by any parameters of each zip code, such as income or density. 

Looking at question 3, how does the population of a zipcode affect gas prices, two figures were generated: a bar graph of the average regular gas price per population of a zip code and a bar graph of the average regular gas price per density of a zipcode. The first figure, Average Gas Price vs Population, has a linear regression line plotted on top of the data, which has an r-squared value of -0.18. This value indicates that there is a weak negative correlation between the population of a zipcode and the prices, meaning that as the population of a zipcode increases, there is a weak correlation that the price of regular gas decreases. This could be because when there is a greater population, the gas station might have a larger amount of customers, which could reduce the price needed for each gas station to create profit. On the other hand, in the second figure, Average Gas Price vs Density, there is a weak positive correlation of the linear regression line of 0.22. This weak positive correlation could be when there is a larger density, which means that the gas station is the closest gas station for more customers, so they can upcharge more.

Looking at question 4, how does the median household income of a zipcode affect gas prices, two figures were generated: the average regular gas price per zip code by median household income in bar graph form as well as in a scatterplot. The first figure, the bar graph, has the zip codes on the x-axis in order of household income. The zipcode with the highest gas prices is 92139, where the household income is 20% of the total median income. The second figure, the scatterplot, has a linear regression line with an r-squared value of 0.03, indicating that there is no correlation between the income of each zip code and the regular gas price.

In addition to these four questions, a figure that shows the map of San Diego with all of the gas stations in our dataset was generated to provide an overall visual of our complete dataset.

  ## Citations
  - The Gas Prices Scraper API, which generated the gas-prices-10-04.csv file, can be found at the following link: https://apify.com/natasha.lekh/gas-prices-scraper
  - The website that generated the Household Income Median.csv file can be found at the following link: https://simplemaps.com/city/san-diego/zips/income-household-median
  - The website that generated the uszips.csv file can be found at the following link: **ADD LINK HERE**
  - The gas_prices_zip_code.ipynb file used code from the website https://stackoverflow.com/questions/25447700/annotate-bars-with-values-on-pandas-bar-plots to annotate bar graphs with the values of each bar in the figure.


