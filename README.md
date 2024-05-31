FINAL PROJECT IRONHACK

SOURCES

Main DataFrame: 
https://www.football-data.co.uk/englandm.php
Ready Dataset
Complemantary Datasets:
www.fbref.com
https://www.worldfootball.net/schedule/eng-premier-league
WebScrapping



Project idea:
EPL Win Predictor and Odds Analyzer
May concentrate to a group of teams (i.e the big 6)


3. Objectives:

Predict Match Outcomes: Develop a machine learning model to predict if a Team is going to win or not a given match.
Compare with Betting Odds: Analyze and compare the predicted probabilities with the odds offered by betting houses to identify discrepancies and value bets.
Provide Insights: Deliver actionable insights to bettors and betting companies for optimizing their strategies and enhancing profitability.


The Notebook: Positionontable_scrapping.ipynb
Scrapes the table with points, matchweek and position on the table

The Notebook: Home&Awaystats.ipynb
Scrapes the data for the Home and Away Team stats for the seasons 2018-2023 (6 in total)

The Notebook: MainTable.ipynb
The main table. Made out on the datasets of the different seasons. Merged here in order to have all the data together and then being able to merge with the other tables.

The Notebook: merges.ipynb
Cleaning the data and also adding some features to all of the 3 tables from the last 2 notebooks.

The Notebook: last_feature_eng.ipynb
Preparing the merged new main table to use it for predictions.
passing some data to newxt rows and converting it to cumulative data. Also performing a couple of more changes so that all the data is numerical.
ensuring the "result" variable is binary. Changing W,L,D to 1 for Win and 0 for L or D.

The Notebook: Logistic_Regression.ipynb
Performed a Logistic Regression.
The model trains the data in the first 5 seasons and tests it on the 2023 season
Evaluating the model. 54% accuracy

The Notebook: Machine_Learning_ModelsEPL.ipynb
RandomForest (didn't performed as well so it was left with unwanted features for prediction like xG or others)
