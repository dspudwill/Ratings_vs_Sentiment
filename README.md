# Does Player Rating Effect Public Sentiment?

**Author:** Dylan Pudwill

**Project Summary:** This project aims to answer how sentiment relates to a players preformance? Mainly, as a playes preformance trends up or down does sentiment move for or against him/her, respectivley? 

## Repo Table of Contents
- README.md (You are here)
    - Summary of project and how its organized in the repository.
- CodeBook.md
    - Overview of orginal data, as well as cleaned varialbes and units.
- pvps.py
    - Python script for building sentiment analysis and player rating data visualizations off of clean data.
- rate_scrape.py
    - Python web scraper that scrapes in data from URL and cleans said data.
- sentiment.py
    - Python API script to pull in sentiment data from social media.
- dataLoad.py
    - Load sentiment and ratings data into database. *Note: Python might not be ideal for this.*
- DbBook.md
    - Overview of data and table organization in the database.

## Overview

This project will have multiple steps.
    
1. Isolate a subset of teams and players to use on this project. They will be selected with a variety of playing levels, team support and social media presence. 

2. Scraping websites to pull in player and team ratings data. The first website to be scraped will be [Whoscored](https://www.whoscored.com/Regions/252/Tournaments/2/Seasons/7811/Stages/17590/PlayerStatistics/England-Premier-League-2019-2) to get player ratings and statistics. To read in team statistics we will try to use two websites: [the Premier League's team statistics site](https://www.premierleague.com/stats), as well as [the Premier League's table site](https://www.premierleague.com/tables). **\[ rate_scrape.py ]**

3. Use Social Media API's(twitter, instagram and facebook) to pull in player & team sentiment data. **\[ sentiment.py ]**

4. Clean Data from scraped URL and send it to the database. **\[ dataLoad.py ]**

5. Take clean data from database and generate data visualizations for output. **\[ pvps.py ]**