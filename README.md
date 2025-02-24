# NBA-Website-Scraping
Code to scrape an NBA statistics website. 

## Project Overview

This project is an NBA game data scraper built with Python. It scrapes game results from the 2023-2024 NBA season for all teams, compiles the data into a pandas DataFrame, and exports it as a CSV file (matches.csv). The data is sourced from Basketball Reference.

How It Works

Scrape Team URLs: The script starts by accessing the NBA standings page and extracting URLs for all team pages in both the Eastern and Western Conferences.

Fetch Game Data: For each team, the script scrapes the list of games, including date, result, score, home/away status, opponent, and team record.

Data Processing: The raw data is cleaned and structured using pandas.

Export to CSV: The final dataset is saved as matches.csv.

