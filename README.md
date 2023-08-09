# web-scraping-challenge
Module 11 Challenge - Data Collection

This project involved the following:
- 1: Scraping titles and preview text from Mars news articles.
- 2: Scraping and analysing Mars weather data, which exists in a table.

Repository Contents:
- part_1_mars_news_kt.ipynb
- part_2_mars_weather_kt.ipynb
- Output:
    - scraped_data_kt.json
    
## Table of Contents

- [About](#about)
- [Getting Started](#getting_started)
- [Installing](#installing)
- [Usage](#usage)
- [Contributing](#contributing)

## About
**Part 1: Scraping titles and preview text from Mars News articles**

Using Splinter and Beauiful Soup libraries in Jupyter Notebook to extract specific data from the Mars News website.

Tools/Libraries Imported:
- splinter library: used for automating web browser actions
- bs4 library: Beautiful Soup, used for parsing websites and scraping specific data
- json libray: to save the exported data in json format
- pathlib library: to create a file path to export the json file to

Jupyter Notebook Python Script:
- File: part_1_mars_news_kt.ipynb
- Purpose:
  - Visit the Mars News Site
  - Scrape the Website for all the text elements
  - Store each title and preview pair in a Python dictionary
  - Store all the dictionaries in a Python list
  - Print the list
  - Export the python list to in a json file (Output/scraped_data_kt.json)

**Part 2: Scraping and analysing Mars weather data, which exists in a table.**

Using Splinter and Beauiful Soup libraries in Jupyter Notebook to extract specific data from the Mars Weather website. Analysis on the data is then performed using Pandas and Matplotlib libraries.

Tools/Libraries Imported:
- splinter library: used for automating web browser actions
- bs4 library: Beautiful Soup, used for parsing websites and scraping specific data
- matplotlib.plplot module: from the matplotlib library, used to create various plots
- pandas library: for data manipulation and analysis

Jupyter Notebook Python Script:
- File: part_2_mars_weather_kt.ipynb
- Purpose:
    1. Visit the Mars Weather Site
    2. Scrape weather data from the main table on the webpage
    3. Create a pandas dataframe from the data
    4. Convert the datatypes of each column for analysis
    5. Analyze the following:
        - How many months are there on Mars?
        - How many Martian days' worth of data are there?
        - What is the average low temperature by month?
        - Plot the average temperature by month
        - Identify the coldest and hottest months in Curiosity's location
        - Average pressure by Martian month?
        - Plot the average pressure by month
        - How many terrestrial (earth) days are there in a Martian year?
    6. Export the data to a CSV file
    7. Close the browser 
        

## Getting Started
To open the files part_1_mars_news_kt.ipynb and part_2_mars_weather_kt.ipynb in Juypter Notebook:
  - Open Anaconda Prompt
  - Activate dev environment, type 'conda activate dev'
  - Navigate to the folder where repository is saved on local drive
  - Open Jupyter Notebook, type 'Jupyter Notebook'
        
## Installing
Need to install the following:
  - Chromedriver (windows x64)
  - Selenium=Beautiful Soup and splinter = automates web browser: pip install "splinter[selenium4]"
  - Beautiful Soup = pip install bs4
  - to parse websites = pip install html5lib
  - to parse websites = pip install lxml

## Usage
A step by step series of examples that tell you how to get a development env running.

## Contributing
Contributors names.
