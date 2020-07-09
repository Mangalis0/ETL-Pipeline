# ETL Pipeline with Scrapping

**Completed by Mangaliso Makhoba.**

**Overview:** In this project we build an ETL Pipeline that will scrape Twitter, that will clean the tweets, convert the them to a Pandas Dataframe then load them to a SQL Server Database

**Problem Statement:** Build ETL for Eskom

**Data:** Tweets

**Deliverables:** ETL Pipeline

## Topics Covered

1. Web Scrapping
3. Data Cleaning
4. Updating SQL Database from Python

## Tools Used
1. Python
1. SQL Server
1. Tweepy
2. PYODBC

## Installation and Usage

Ensure that the following packages have been installed and imported.

```bash
pip install numpy
pip install pandas
pip install pyodbc
pip install tweepy
```

#### Jupyter Notebook - to run ipython notebook (.ipynb) project file
Follow instruction on https://docs.anaconda.com/anaconda/install/ to install Anaconda with Jupyter. 

Alternatively:
VS Code can render Jupyter Notebooks

## Notebook Structure
The structure of this notebook is as follows:

1. Function to connect to twitter and scrapes "Eskom_SA" tweets.
<br>
<br>
2. Cleans/Processes the tweets from the scraped tweets which will create a dataframe with two new columns using the following functions: <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; a) Hashtag Remover from Analyse Functions
<br>
<br>
3. Functions which connects SQL database and uploads the tweets into the table you store the tweets in the database.



# Function 1: Scrapping Twitter

Write a function which:
- Scrapes _"Eskom_SA"_ tweets from Twitter. 

Function Specifications:
- The function should return a dataframe with the scraped tweets with just the "_Tweets_" and "_Date_". 
- Will take in the ```consumer key,  consumer secret code, access token``` and ```access secret code```.

NOTE:
The dataframe should have the same column names as those in your SQL Database table where you store the tweets.


# Function 2: Removing hashtags and the municipalities

Write a function which:
- Uses the function you wrote in the Analyse section to extract the hashtags and municipalities into it's own column in a new data frame. 

Function Specifications:
- The function should take in the pandas dataframe you created in Function 1 and return a new pandas dataframe.

# Function 3: Loading Data to SQL Server
Write a function which:
- Connects and updates your SQL database. 

Function Specifications:
- The function should take in a pandas dataframe created in Function 2. 
- Connect to your SQL database.
- Update the table you store your tweets in.
- Not return any output.


## Conclusion
This notebook can be modified by changing the parameters to suit your databse. 

## Contributing Authors
**Authors:** Mangaliso Makhoba, Explore Data Science Academy

**Contact:** makhoba808@gmail.com

## Project Continuity
This is project is complete

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. 

## License
[MIT](https://choosealicense.com/licenses/mit/)
