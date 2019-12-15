# hernanCortez
Repository for Hernan Cortez

In sentimentAnalysis.zip you will find the entirety of my project progression for my independent study 
course with Mark McKenney at SIUE Fall 2019. 

You will find a py folder containing my whole project that consists of .py, .txt, .csv, and .html files.

********** .py files **********************************************************************************************
twtQuery.py
This file was used to filter and focus my query for tweets with subject matter relating to my topic.
You can manipulate filters, keywords for phrases you plan to search for, geo-location of tweet, maximum
number of tweets, etc. Everytime this file runs it will output two files, one .txt and one .csv, containing
the same data for the tweets meeting your criteria. This files are saved in the data folder.

twtSentimentAnalysis.py
This file uses python's VADER sentiment analysis tool to analyze the found tweets. It reads in the .csv files
produced from twtQuery.py, runs tweets through VADER sentimetn analysis tool, and makes a copy of the passed
in .csv files in addition to adding sentiment score data columns and adding color columns based on scores.
These newly produced .csv files are stored in the processedData folder

twtPlot.py
This file reads in the .csv files stored in the processedData folder and plots each tweet as a marker on a
folium map. It colors in each marker according to the sentiment scores produced from twtSentimentAnalysis.py
file. The map that is created using python's folium package is stored as tweets.html.
*******************************************************************************************************************


********* .txt files **********************************************************************************************
immigrants 12-2-19.txt
immigration 12-1-19.txt
keywords.txt
These files contain data gathered from tweets I queried. These files helped me debug and troubleshoot my .py files.

latestIDTracker.txt
This file helped me keep track of latest tweet ID I had queried at the time.

middle of the united states.txt
This file contains data from what I presumed to be the middle of the U.S. which helped me limit the scope of the 
queried tweets
*******************************************************************************************************************


********** .csv files *********************************************************************************************
immigrants 12-2-19.csv
immigration 12-1-19.csv
keywords.csv
These are the set of .csv files produced by twtQuery.py.

immigrants 12-2-19 (processed).csv
immigration 12-1-19 (processed).csv
keywords (processed).csv
These are the set of .csv files produced by twtSentimentAnalysis.py. These contain the data requried to ploy the 
folium map.
*******************************************************************************************************************


********** .html file *********************************************************************************************
tweets.html
This file contains the folium map produced by twtPlot.py. 
*******************************************************************************************************************








