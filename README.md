# Predicting the Outcomes of NFL Games
<img src='https://i.imgur.com/98xMf7J.jpg'>

I'll be attempting to predict the outcome of NFL games using game data from the past 3 years(2017-2019). I trained my models on known game data and in order to make predictions, I used the averages of the past 3 games each team has played. 

## Data Source

I gathered all my data from https://www.footballdb.com using box scores for each game to gather game data.
After acquiring the data, I cleaned it up and converted it into csv files which can be found in the data folder.
The data cleaning process that I used can be found in the Data Gathering notebook.

## Models used for predictions

I'll be running the prediction data through a couple different models to see which one yields the best results. 

The models I'll be using are:<br>
* Logistic Regression
* Support Vector Machine
* Random Forest
* XGBoost

<img src='https://i.imgur.com/B3827An.png'>

The home team wins their games 56% of the time, so I'm looking for an accuracy rate greater than 56%

## Logistic Regression

### Evaluation Metrics

Precision:  65% <br>
Recall:  51% <br>
Accuracy:  57% <br>
F1-Score:  57% <br>

<img src='https://i.imgur.com/Y2HmeLZ.png'>

## Support Vector Machine

### Evaluation Metrics

Precision:  66% <br>
Recall:  60% <br>
Accuracy:  60% <br>
F1-Score:  63% <br>

<img src='https://i.imgur.com/D3XWnnE.png'>

## Random Forest

### Evaluation Metrics

Precision:  63% <br>
Recall:  62% <br>
Accuracy:  58% <br>
F1-Score:  63% <br>

<img src='https://i.imgur.com/Ke3l65G.png'>

## XGBoost

### Evaluation Metrics

Precision:  66% <br>
Recall:  62% <br>
Accuracy:  60% <br>
F1-Score:  64% <br>

<img src='https://i.imgur.com/Z06ezpV.png'>

## Conclusion

While the outcome of games that have already been played can be predicted at a very high percentage (above 85%), the same cannot be said for predicting the outcome of future games. In order to predict the outcome of future games, I used the averages of the previous 3 weeks for each team and ran that data through various models to determine which model performed the best with the data. The XGBoost model performed the best of the models I tested and I am able to predict the outcome of an NFL game with an accuracy of 60%. 