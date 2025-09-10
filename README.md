##Premier League Data Analysis and Prediction Project
##Overview
##This project consists of two main components:

Web Scraping & Data Processing: A Jupyter Notebook that scrapes Premier League data from FBref.com and processes it into a structured format

Prediction & Visualization: Python code that analyzes the processed data to predict next season's winner and creates visualizations

##Web Scraping Notebook (webscraping.ipynb)
Purpose
This notebook collects and processes Premier League football statistics from FBref.com for both the 2023-2024 and 2024-2025 seasons.

##Key Steps
Import Libraries: Uses pandas for data manipulation

Data Collection:

Scrapes current season standings from FBref

Collects squad statistics for both 2024 and 2025 seasons

Data Processing:

Filters and selects relevant columns (Rank, Squad, Points, Wins, Draws, Losses, Goal Difference, Goals For, Goals Against, Expected Goals)

Processes squad statistics including number of players, average age, and possession percentage

Merges standings data with squad statistics for both seasons

Data Export:

Saves the processed data to a CSV file (premier_league_standings_filtered.csv)

##Output
Creates a comprehensive dataset with the following columns for each team:

Current season performance metrics (Points, Wins, Goals, etc.)

2024 squad characteristics (Number of players, Average age, Possession %)

2025 projected squad characteristics

##Prediction & Visualization Code
Purpose
Analyzes the processed data to predict the winner of the next Premier League season and creates visualizations to support the analysis.

##Key Steps
Data Loading & Preparation:

Loads the processed CSV data

Filters teams with complete 2025 data

Calculates year-over-year changes in squad characteristics

##Prediction Model:

Uses Linear Regression with multiple factors:

Current Points (Pts)

Goal Difference (GD)

Expected Goals (xG)

2025 Squad Age

2025 Possession Percentage

Adds randomness to simulate uncertainty in predictions

##Visualization:

Creates four comprehensive plots:

Current vs Predicted Points comparison

Key metrics for top teams (Goal Difference, Possession, Expected Goals)

Squad age comparison between 2024 and 2025

Predicted standings for next season

##Results:

Identifies Liverpool as the predicted winner for next season

Provides detailed comparison of top contenders

Outputs full predicted standings table

##Key Features
Uses machine learning (Linear Regression) for prediction

Incorporates multiple performance metrics

Provides visual evidence to support predictions

Highlights Liverpool's strengths: dominant current performance, strong goal difference, and sustainable attacking metrics

##How to Use
Run the Jupyter Notebook to scrape and process the latest data

Execute the prediction code to generate analysis and visualizations

Review the visualizations to understand team performance and predictions

##Dependencies
pandas

numpy

matplotlib

seaborn

scikit-learn

Jupyter Notebook

##Data Sources
All data is scraped from FBref.com, a comprehensive football statistics website.

Note
The prediction model is based on historical performance metrics and projected squad characteristics, but actual football results can be influenced by many unpredictable factors.
