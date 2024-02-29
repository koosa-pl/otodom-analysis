# otodom-analysis
Analysis of sample data scraped from otodom.pl website.

## Readme/Documentation

The goal of this project was to look into and gain some insights about the real estate market in Poland. The sample dataset with 1000 records was downloaded from brightdata.com which offers many up-to-date, business-ready datasets scraped from popular websites. The particular dataset used in this project was scraped by brightdata from site otodom.pl which is a major website for posting real estate advertisements in Poland. The dataset contains information about advert’s title, property’s surface(in meters squared), price (in PLN), number of rooms and other.

The SQL queries used in Snowflake along with tables and visualizations can be found in the **otodom-analysis.pdf** or **otodom-analysis.html**. file.

Below are the steps taken for the project:

1. Downloaded the sample data from brightdata (**Otodom Poland.csv**)
2. Created a python script for translating advert titles from Polish to English, using the deep_translator module from PyPi. The script is located in **title_translator.ipynb** file.
3. Loaded the data into Snowflake Data Cloud. Not all records could have been loaded due to errors, in result Snowflake loaded 985 records out of 1000.
4. Created additional columns for dividing advert locations into ten most populated cities in Poland as "major city" and the other as "smaller city". Also, created another columns for those ten distinct cities for further analysis.
6. Run the queries in Snowflake, created visualizations with built-in chart generator. All used queries can be found in **otodom_queries.txt** file.
7. Collected queries and visualizations into **otodom-analysis.html** file made with RMarkdown editor in RStudio. The original RMarkdown code can be found in **otodom-analysis.Rmd** file.
