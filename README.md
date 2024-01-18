# Trading Strategy - Foreign Exchange Rate Analysis Project

This project involves scraping foreign exchange rate data, implementing a trading strategy based on the scraped data, and observing the overall results.

## Project Flow

1. **Data Scraping**: The 'Final - Data Scraper' script is used to scrape foreign exchange rate data for various currency pairs using the Polygon.io API.

2. **Data Storage**: The scraped data is stored in CSV files, each named according to the currency pair (e.g., 'currency_pair.csv').

3. **Trading Strategy Implementation**: The stored data is used to implement a trading strategy through several scripts, including 'USDGBP Results', 'Strategy [Live Data] - 2', and 'Strategy [Live Data] - 3'. These scripts analyze the foreign exchange rates for specific currency pairs, calculate returns, and implement a trading strategy based on certain conditions.

4. **Results Observation**: The overall results of the trading strategy are observed, assessing its performance and effectiveness.

5. **Presentation**: All the details and findings of the project are compiled and presented in a PowerPoint file named 'Final Presentation.pptx'.

## Libraries Used
- pandas
- numpy
- matplotlib.pyplot

## Note

The scripts require the respective CSV files to run. Make sure these files are in the same directory as the scripts.

## Disclaimer

This project is for educational purposes only. Always ensure you have the necessary permissions and understand the potential implications when dealing with financial data.

## Final - Data Scraper

This Python script fetches and tracks foreign exchange rates for 10 currency pairs using the Polygon.io API.

### Libraries Used
- requests
- numpy
- warnings
- pandas
- datetime
- sqlite3
- sqlalchemy
- seaborn
- time

### How it Works

The script uses the Polygon.io API to fetch the current exchange rate for 10 different currency pairs (USD to GBP, INR, JPY, CAD, EUR, TRY, RUB, MXN, AUD, CNY). The data is fetched every 0.75 seconds for a maximum of 5 hours.

The fetched data includes the conversion rate and timestamp, which are then stored in a pandas DataFrame. The timestamp is converted from Unix time to a more readable format.

The script now includes additional code for the USD to INR, USD to JPY, USD to CAD, USD to EUR, USD to TRY, USD to RUB, USD to MXN, USD to AUD, and USD to CNY currency pairs. The new code fetches the conversion rate and timestamp for these pairs, stores them in a DataFrame, and converts the timestamp to a more readable format.

The script also exports the currency pair data to a CSV file named "usd_$abc_final.csv".

### Note

Please replace the `apiKey` in the API URLs with your own Polygon.io API key.

## USDGBP Results [Live Data], # Strategy [Live Data] - 2, # Strategy [Live Data] - 3

These Python scripts analyze the foreign exchange rates for the USD to another currency pair.

### Libraries Used
- pandas
- numpy
- matplotlib.pyplot

### How it Works

The script reads the data from a .CSV file named "usd_$abc_final.csv" and calculates the returns for each data point. It then calculates the average return, average price, and standard deviation for every 360 data points.

The script also implements a simple trading strategy: if there are 3 consecutive positive returns, it triggers a sell; if there are 3 consecutive negative returns, it triggers a buy. If these conditions aren't met, it does nothing.

The script creates a DataFrame that includes the average price, standard deviation, average return, and trading decision for each set of 360 data points.

The script then calculates the profit from the trading strategy and plots the Bollinger Bands for the average prices.

The script also calculates the total number of trades conducted and the total number of trades conducted outside the Bollinger Bands.

### Note

The script requires the "usd_$abc_final.csv" file to run. Make sure this file is in the same directory as the script.
