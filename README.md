# otodom-analysis
Analysis of sample data scraped from otodom.pl website.

# Readme/Documentation

The goal of this project was to look into and gain some insights about the real estate market in Poland. The sample dataset with 1000 records was downloaded from brighdata.com which offers many up-to-date, business-ready datasets scraped from popular websites. The particular dataset used in this project was scraped by brightdata from site otodom.pl which is a major website for posting real estate advertisements in Poland. The dataset contains information about advert’s title, property’s surface(in meters squared), price (in PLN), number of rooms and other.

The insights of the project along with used queries and visualizations can be found in the …. file

Below are the steps for the project:

Downloaded the sample data from brightdata (Otodom Poland.csv)
Created a python script for translating advert titles from Polish to English, using the deep_translator module from PyPi. The script is located in title_translator.ipynb file.
Loaded the data into Snowflake Data Cloud. Not all records could have been loaded due to errors, in result Snowflake loaded 985 records out of 1000.
Run the queries in Snowflake, created visualizations with built-in chart generator.
Collected queries, visualizations and insights into … file.
