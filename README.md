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

I used Splinter and Beauiful Soup libraries in Jupyter Notebook to scrape and extract weather data from the Mars Weather website that was in a table. As done in Part 1 above, in order to identify the data to extract, I opened the website in my Chrome web brower, then selected the 'Developer Tools' (Ctrl+Shift+I). Upon inspecting the html code, I was able to identify the section of code corresponding to the data in the table on the page. I created an empty list which would then be filled with the data from the table, by looping through each row and column. Once I had the list of rows, and the list of column names, using the Pandas library, I formed a dataframe. 

Before I performed any analysis, I converted the datatypes of each column eg. from Object to integer or float, depending on the column data. I was then able to perform various types of analysis using Pandas and Matplotlib libraries. Finally, I exported the dataframe to a csv file in an 'Output' folder and closed the browser.

Tools/Libraries I Imported:
- splinter library: used for automating web browser actions
- bs4 library: Beautiful Soup, used for parsing websites and scraping specific data
- matplotlib.plplot module: from the matplotlib library, used to create various plots
- pandas library: for data manipulation and analysis

My Files:
- Jupyter Notebook Python Script: part_2_mars_weather_kt.ipynb
- csv file: Output/mars_temperature_data.csv       

## Getting Started
To open the files part_1_mars_news_kt.ipynb and part_2_mars_weather_kt.ipynb in Juypter Notebook:
  - Open Anaconda Prompt
  - Activate dev environment, type 'conda activate dev'
  - Navigate to the folder where repository is saved on local drive
  - Open Jupyter Notebook, type 'Jupyter Notebook'
        
## Installing
I installed the following:
  - Chromedriver (windows x64) (go to: https://googlechromelabs.github.io/chrome-for-testing/#stable, select a stable version of Chromedriver that is suitable for your pc. Unzip the files and make sure that the folder path containing the files is added to Environment Variables > Path on your pc.)

Open 'Anaconda Prompt', activate dev environment (see Getting Started section above), then install the following:
  - Splinter library with optional dependency Selenium to automate tasks on websites, type: pip install "splinter[selenium4]"
  - Beautiful Soup library for web scraping, type: pip install bs4
  - html5lib library to parse websites, type: pip install html5lib


