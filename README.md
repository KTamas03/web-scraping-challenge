# web-scraping-challenge
Module 11 Challenge - Data Collection

In this project, the main challenge involved collecting data from websites by using web scraping. The two websites were:

- Mars News:
    - https://static.bc-edx.com/data/web/mars_news/index.html
    - I scraped information from a list of news articles
- Mars Weather:
    - https://static.bc-edx.com/data/web/mars_facts/temperature.html
    - I scraped weather information from a table. Then I performed some analysis on the scraped table data

Repository Contents:
- part_1_mars_news_kt.ipynb
- part_2_mars_weather_kt.ipynb
- Output:
    - scraped_data_kt.json
    - mars_temperature_data.csv
    
## Table of Contents

- [About](#about)
- [Getting Started](#getting_started)
- [Installing](#installing)
- [Usage](#usage)
- [Contributing](#contributing)

## About
**Part 1: Scraping titles and preview text from Mars News articles**

I used Splinter and Beauiful Soup libraries in Jupyter Notebook to scrape and extract text containing the title and preview of each article listed on the Mars News website. In order to identify which text to extract, I opened the website in my Chrome web brower, then selected the 'Developer Tools' (Ctrl+Shift+I). Upon inspecting the html code, I was able to identify the section of code corresponding to the title and preview pairs of each article listed on the page.

Each title and preview pair were then stored in a python dictionary. Then I stored all of the dictionaries in a python list. Lastly, I exported the dictionary in a json format file in an 'Output' folder and closed the browser.

Tools/Libraries I Imported:
- splinter library: used for automating web browser actions
- bs4 library: Beautiful Soup, used for parsing websites and scraping specific data
- json libray: to save the exported data in json format
- pathlib library: to create a file path to export the json file to

My Files:
- Jupyter Notebook Python Script: part_1_mars_news_kt.ipynb
- JSON file: Output/scraped_data_kt.json)

**Part 2: Scraping and analysing Mars weather data, which exist in a table.**

I used Splinter and Beauiful Soup libraries in Jupyter Notebook to scrape and extract weather data from the Mars Weather website that was in a table. I created an empty list which would then be filled with the data from the table, by looping through each row and column. Once I had the list of rows, and the list of column names, using the Pandas library, I formed a dataframe. 

Before I performed any analysis, I converted the datatypes of each column eg. from Object to integer or float, depending on the column data. I was then able to perform various types of analysis on the data using Pandas and Matplotlib libraries. Finally, I exported the dataframe to a csv file in an

Tools/Libraries I Imported:
- splinter library: used for automating web browser actions
- bs4 library: Beautiful Soup, used for parsing websites and scraping specific data
- matplotlib.plplot module: from the matplotlib library, used to create various plots
- pandas library: for data manipulation and analysis

My Files:
    - Jupyter Notebook Python Script: part_2_mars_weather_kt.ipynb
    - csv file: Output/mars_temperature_data.csv

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
