# Prague airbnb price prediction project
This project aims to accurately predict price per night in Prague using advanced data analytics techniques.

Authors: Team 2

Data source: http://insideairbnb.com/get-the-data/
(Detailed Listings data, Detailed Calendar Data, Detailed Review Data)

Data dictionary: https://docs.google.com/spreadsheets/d/1iWCNJcSutYqpULSQHlNyGInUvHg2BoUGoNRIGa6Szc4/edit#gid=1322284596 

## Technologies
Python 3 - programming language used, done in Visual Studio code and Jupyter Notebook.

## Prerequisites
Install the required packages in your terminal or set up your virtual enviroment.

pip3 install -r requirements.txt

## Preprocessing
Dataset: detailed Listings data for Prague

Jupyter_preprocessing

  Some changes in dataset prior to modeling: 
- Elimination of NA observation for variable price
- Calculate correlation between all variables
- Create dummy variables for categorical variables
- Logarithmic transformation of the price variable 
- Handling NA values through interpolation
- Identify and handle outliers – based on standard deviation

## Models
Dataset: data_cleaned from preprocessing

Jupyter_regression
- sklearn_model, GridSearchCV, RFE + GridSearchCV, ridge_model, lasso_model
  
Jupyter_trees
- Random Forest (bez CV),  Random Forest (s CV), Random Forest (truncated),   XGBoost,  XGBoost (s CV) 
  
## Bonus
Dataset: detailed Calendar Data, detailed Review Data for Prague

Jupyter_bonus

1. Sentiment analysis - relation between the sentiment and price, Were people who paid more also more satisfied?
2. Seasons - What high seasons did you identify? 
