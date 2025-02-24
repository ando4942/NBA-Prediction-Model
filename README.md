# NBA Game Data Scraper and Prediction Model
Code to scrape data from website and train a model to predict games.

## Project Overview

This project involves scraping NBA game data from the 2023-2024 season using Python and building a machine learning model to predict game outcomes. The project uses web scraping, data processing, and a Random Forest Classifier to predict whether a team will win or lose a match based on historical data.

Components
Data Scraping: Utilizes BeautifulSoup and Requests to scrape game data from Basketball Reference.
Data Processing: Cleans and organizes the scraped data using pandas.
Prediction Model: Implements a Random Forest Classifier with scikit-learn to predict game results.
Evaluation: Measures accuracy and precision of the model and outputs a confusion matrix.

### How It Works
#### Data Scraping
- Scrapes team URLs from both Eastern and Western Conference standings.
- Extracts game details including date, result, score, home/away status, opponent, and team record.
- Saves the cleaned data to matches.csv.
#### Prediction Model
The model uses the following features:
- venue_code: Encodes whether the game was at home or away.
- opp_code: Categorical encoding of the opponent team.
- day_code: Day of the week of the game.
- month: Month of the game.
Trains the model on data before 2024 and tests it on 2024 data. Uses accuracy and precision as evaluation metrics.
