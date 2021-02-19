# Flight-Fare-Predction-App

This application tell us about the Fare of flight .

The App Link :    https://flight-price-predction-ml-app.herokuapp.com/

Application Video link :   https://drive.google.com/file/d/1ZUmiqKlnXbiQRqVKEpiKNNe_2zE3BjN1/view?usp=sharing

Some Glimpses of Application : 

![rcd1](https://user-images.githubusercontent.com/61588604/108451141-51e6cc00-728c-11eb-90c7-969af53c94b8.png)

![rcd2](https://user-images.githubusercontent.com/61588604/108451179-62974200-728c-11eb-981b-87f5e7383a34.png)

![rcd3](https://user-images.githubusercontent.com/61588604/108451237-78a50280-728c-11eb-806c-7b23e518f539.png)



Journey : 

1) Data Collection :  Data collected from the Kaggle . 
    about data : Data COlumns are : mid(match number) ,date, venue, bat_team, bowl_team , batsman, bowler, runs, wickets, overs, run_last_5(runs made in last 5      overs),wickets_last_5(wickets taken in last 5 overs), non_striker and total score of that match .
    
    As a data scientist, we will predict the total predicted score for first inning when user give some input .(input : select teams for batting and bowling and current runs , wickets and overs  and runs & wickets in last 5 overs .)
    
    Assumption : all batsman and bowlers have same capability and  there is no effect of venue)
    
2) Data Preprocessing : 
    first of all , deleted all unused columns(mid,date,venue,batsman ,bowler) from dataset. and cleaned from null values.
    
    then I used one-hot-encoding for "bat_team" and "bowl_team" columns.
    
3) Model building : 
    a) split the dataset into X(independent features) and y(dependent features) .
    b) perform train_test_split
    c) try linear regression , lasso regression, ridge regression, RandomForestRegressor with hyperparameter tuning. 
    d) obsered that linear regression has highest score and lowest error . so save this model using pickle.

4) Model deployment : 
    a) using flask framework , we deployed this model on HEROKU platform .
    
App link : https://ipl-score-prediction-akd-app.herokuapp.com/
    
    
