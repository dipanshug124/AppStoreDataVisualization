# app-store-data-viz
Data visualization of app store data, needed by game developer to create app with better ratings.

## Objective
To expose the best combination for strategy games available in the AppStore in order to get a good user rating (4.0/5.0 and above).

#### Downloading data
Dataset is found on [kaggle.com](https://www.kaggle.com/tristan581/17k-apple-app-store-strategy-games)
(I've also added it here as [appstore_games.csv](https://github.com/dipanshug124/app-store-data-viz/blob/master/appstore_games.csv)

**Data Cleaning**  
* Games without User Rating are dropped.
* Games with less than 200 user rating AND days since last update date <6month are dropped to prevent biased ratings from the developer
* Genre tags "Entertainment" and "Games" are removed from the Genre string as it does not provide meaningful insight
* The remaining of the string are checked and grouped as follows:  
    Puzzle= Puzzle/Board  
    Adventure= Adventure/Role/Role Playing  
    Action = Action  
    Family = Family/Education

**Libraries**
* `Numpy` :http://www.numpy.org/
* `Pandas` :http://pandas.pydata.org
* `matplotlib` :http://matplotlib.org/
* `seaborn` :https://seaborn.pydata.org
* `Datetime` :https://docs.python.org/3/library/datetime.html
*  `Statistics` :https://docs.python.org/3/library/statistics.html

**Software Recommended**
* [Jupyter Notebook](http://ipython.org/notebook.html)
* [Anaconda](http://continuum.io/downloads) installed with `Python 3.8`

## Summary  
Final code is uploaded in [data_viz](https://github.com/dipanshug124/app-store-data-viz/blob/master/data_viz.ipynb)  
Using different graphs and piecharts we can ananlyze and make inferences on the data.

![](https://github.com/dipanshug124/app-store-data-viz/blob/master/Graphs/1.png)
![](https://github.com/dipanshug124/app-store-data-viz/blob/master/Graphs/3.png)
![](https://github.com/dipanshug124/app-store-data-viz/blob/master/Graphs/4.png)
![](https://github.com/dipanshug124/app-store-data-viz/blob/master/Graphs/6.png)
![](https://github.com/dipanshug124/app-store-data-viz/blob/master/Graphs/7.png)
![](https://github.com/dipanshug124/app-store-data-viz/blob/master/Graphs/8.png)
![](https://github.com/dipanshug124/app-store-data-viz/blob/master/Graphs/download.png)
![](https://github.com/dipanshug124/app-store-data-viz/blob/master/Graphs/images)

**Genre grouping**  
* Puzzel has less average rating comparing to other Genres.  
* Action & Adventure Genre games above 600MB have more tendency to achieve rating 4.0 and above.  
* Family Games show lesser rating with size above 200MB.  

**Game Size Analysis**  
* Games below 250MB -> focus on size between 100MB to 150MB of contents.  
* Games between 250MB to 1GB -> focus on size between 500MB+ of contents.  

**Release Date/ Update Factor**  
* Almost 90% of the developers focuses on games below 1 Dollar and places In-App Purchase as their strategy for income.  

**Game price and In-App Purchase Factor**  
* A large number of Developers create free games.  
* Puzzel shows more no. of paid players compare to others.  

**Age Rating Factor**  
* Games with age rating 12+ gains more likes.


