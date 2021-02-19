# Flight-Fare-Predction-App

This application tell us about the Fare of flight .

The App Link :    https://flight-price-predction-ml-app.herokuapp.com/

Application Video link :   https://drive.google.com/file/d/1ZUmiqKlnXbiQRqVKEpiKNNe_2zE3BjN1/view?usp=sharing

Some Glimpses of Application : 

![rcd1](https://user-images.githubusercontent.com/61588604/108451141-51e6cc00-728c-11eb-90c7-969af53c94b8.png)

![rcd2](https://user-images.githubusercontent.com/61588604/108451179-62974200-728c-11eb-981b-87f5e7383a34.png)

![rcd3](https://user-images.githubusercontent.com/61588604/108451237-78a50280-728c-11eb-806c-7b23e518f539.png)



Journey : 

**1) Data Collection** :  Data collected from the Kaggle . 
    **about data** : Data Columns are : Airline ,Date_of_journey, Source, Destination, Route , Dep_Time, Arrival_Time, Duration, Total_Stop, Additional_info,Price . 
    
    As a data scientist, we will predict the total predicted Fare for flight when user give some input .(input : Departure_Date, Arrival_Date, Source, Destination, number_of_stops and airline_type .)
    
    
**2) Data Preprocessing :** 
        The major thing in this project is "Dat daa Preprocessing " only ,because there are all columns of categorical-type and some are string but actually they are "Date" columns .
        
        a)Date_of_Journey is a object data type, Therefore, we have to convert this datatype into timestamp so as to use this column properly for prediction.
        we use datetime and fetch day and month and made two seperate columns named as "Journey_day" and "Journey_month" and deleted "Date of journey" column.
        
        b)
        
        

    
3) Model building : 
    a) split the dataset into X(independent features) and y(dependent features) .
    b) perform train_test_split
    c) try linear regression , lasso regression, ridge regression, RandomForestRegressor with hyperparameter tuning. 
    d) obsered that linear regression has highest score and lowest error . so save this model using pickle.

4) Model deployment : 
    a) using flask framework , we deployed this model on HEROKU platform .
    
App link : https://ipl-score-prediction-akd-app.herokuapp.com/
    
    
