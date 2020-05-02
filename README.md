# app-store-data-viz
Data visualization of app store data, needed by game developer to create app with better ratings.


This is a data visualtion of games of different types. Dataset is found on [kaggle.com](https://www.kaggle.com/tristan581/17k-apple-app-store-strategy-games)

###Data Cleaning  
* Games without User Rating are dropped.
* Games with less than 200 user rating AND days since last update date <6month are dropped to prevent biased ratings from the developer
* Genre tags "Entertainment" and "Games" are removed from the Genre string as it does not provide meaningful insight
* The remaining of the string are checked and grouped as follows:  
    Puzzle= Puzzle/Board  
    Adventure= Adventure/Role/Role Playing  
    Action = Action  
    Family = Family/Education
