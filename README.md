# Project1

Project by Vanessa Dumlao, Shruti Palur Mallampalli, and Noelle Watson

## Overview
The Project 1 Repository consists of data pertaining to gas prices in San Diego. The project explores gas prices in San Diego to see how factors such as zip code, household income, and population density affect these prices. 

The repository contains the Resource folder, which contains two csv files that hold all of the source data. Also in the Resource folder are two csv files which were created using the gas_price_zip_code.ipynb file. 

Outside of the Resource folder are two Jupyter Notebook files, the gas_price_zip_code.ipynb script, and the charts.ipynb script. The gas_price_zip_code.ipynb takes the source data from two csv files and combines them according to zip code, and outputs the Zip Code All Data.csv file. The script also outputs the extra_clean_gas.csv which has the cleaned data from the gas-prices-10-04.csv file. The charts.ipynb script takes the outputted csv files analyzes the data, and produces various charts.

## Data Source and Gathering
The data used in Project 1 comes from two different sources. The second set of data, which can be found in gas-prices-10-04.csv, was generated by Gas Prices Scaper, an api that collects that day’s current gas prices at every gas station whose prices are listed on google maps within the search parameters. The data within gas-prices-10-04.csv comes are the gas prices from October 4, 2023. The area in which data was collected for, was determined by the zip codes that were available in the Household Income Median.csv file. The Household nNcome Median.csv file was generated from simplemaps.com for the area of San Diego.

## Overview of printed figure
In the charts.ipynb file, the extra_clean_gas.csv file and the Zip Code Data All.csv file were analyzed, and eight figures were generated in response to _four questions_:

1. How are zipcodes and gas prices affected by gas station brands?
2. How does zipcode affect differnces in gas prices between types?
3. How does population of a zipcode affect gas prices?
4. How does the median household income of a zipcode affect gas prices?

Looking at question 1, how are zipcodes and gas prices affected by gas station brands, two figures were generated: a stacked bar graph of brands by zip code, and a bar graph of the average gas price by gas station brands. From the two figures, it can been see that the number of brands of gas stations in zip codes vary from 1 to 9, and that the average price of gas by brand ranges from $5.70 to $6.50 USD/gallon. Based on the two figures together, it does not seem that zipcodes and gas prices are affected by gas station brands.

Looking at question 2, how does zipcode affect differnces in gas prices between types, two figures were generated, a stacked line plot of Regular, Midgrade, and Premium gas prices per zipcode, and a stacked scatterplot of Regular, Midgrade, and Premium gas prices per zipcode that were ordered by average income. From the first figure, Gas Prices Per Type vs. Zip Code, each line for the different types of gases are extremly similar to each other, with the gaps ranging from $0.10 to $0.20. The third figure, Gas Price per Type vs Average Income per Zip Code, is the a scatterplot of the gas price for each type of gas is ploted against the income of each zipcode, with a linear regression line plotted for each gas type. The slope for all three types of gas is very small, to the order of negative seven, and all similar to each other, indicating that the differnence of price between the types of gas is not affected by any parameters of each zipcode such as income or density. 

Looking at question 3, how does population of a zipcode affect gas prices, two figures were generated: a bar graph of the average regular gas price per population of a zipcode, and a bar graph of the average regular gas price per density of a zipcode.

Looking at question 4, how does the median household income of a zipcode affect gas prices, two figures were generated: the average regular gas price per zip code by median household income in bar graph form as well as in a scatterplot.

In addition to these four questions, a figure that shows the map of San Diego with all of the gas stations in our dataset was generated to show provide an overall visual of our complete dataset.

  
  ## Citations
  - The Gas Prices Scraper api which generated the gas-prices-10-04.csv file can be found at the following link: https://apify.com/natasha.lekh/gas-prices-scraper
  - The website that generated the Household Income Median.csv file can be found at the following link: https://simplemaps.com/city/san-diego/zips/income-household-median
  - The gas_prices_zip_code.ipynb file used code from the website: https://stackoverflow.com/questions/25447700/annotate-bars-with-values-on-pandas-bar-plots, to annotate bar graphs with the values of each bar in the figure.


