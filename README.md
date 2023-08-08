# web-scraping-challenge
Module 11 Challenge - Data Collection

This project involved the following:
- 1: Scraping titles and preview text from Mars news articles.
- 2: Scraping and analysing Mars weather data, which exists in a table.

UPDATE Repository Folders and Contents:
- SurfsUp:
  - Resources:
    - hawaii.sqlite
    - hawaii_measurements.csv
    - hawaii_stations.csv
  - app.py
  - climate_kt.ipynb
    
## Table of Contents

- [About](#about)
- [Getting Started](#getting_started)
- [Installing](#installing)
- [Usage](#usage)
- [Contributing](#contributing)

## About
**Part 1: Scraping titles and preview text from Mars news articles**

Python and SQLAlchemy are used to do a basic climate analysis and data exploration of the climate database. Specifically, SQLAlchemy ORM queries, Pandas, and Matplotlib.ct are used.

Tools/Libraries Imported:
- matplotlib.pyplot library: used for creating graphs and charts
- matplotlib style 'fivethirtyeight': specific plot style with predefined colours, and fonts
- numpy library: used for numerical computations
- pandas library: used for data manipulation and analysis
- datetime library: provides classes for manipulating dates and times


Jupyter Notebook Python Script:
- File: climate_kt.ipynb
- Purpose:
  - Use sqlalchemy to connect to the hawaii.sqlite database
  - Reflect the tables from the database into classes and save references to them, named 'station' and 'measurement'
  - link Python to the hawaii.sqlite database by creating a sqlalchemy session
      
## Getting Started
To open climate_kt.ipynb in Juypter Notebook:
  - Open Anaconda Prompt
  - Activate dev environment, type 'conda activate dev'
  - Navigate to the folder where repository is saved on local drive
  - Open Jupyter Notebook, type 'Jupyter Notebook'

To open app.py and activate the flask API:
 - Open app.py in Visual Studio Code
 - Navigate to the folder location of the app.py file where it is saved on the local drive
 - In the Terminal type 'python app.py'
 - The url should be http://127.0.0.1:5000:
      - open a webpage with the above url
      - add the different routes to see the JSON output eg. http://127.0.0.1:5000/api/v1.0/precipitation
      - to close the flask app in Visual Studio Code, press Ctrl + c
        
## Installing
Need to install the following:
  - Chromedriver
  - Selenium=Beautiful Soup and splinter = automates web browser: pip install "splinter[selenium4]"
  - Beautiful Soup = pip install bs4
  - to parse websites = pip install html5lib
  - to parse websites = pip install lxml

## Usage
A step by step series of examples that tell you how to get a development env running.

## Contributing
Contributors names.
