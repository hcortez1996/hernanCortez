# hernanCortez
Repository for Hernan Cortez

twtQuery.py
Used to query tweets that included various filters such as geo-tag and keywords.

twtLDA.py
Used gensim's LDA to derive the desired number of topics from the queried tweets. 
Also, uses pyLDAvis for visualization of LDA topics and outputs wordclouds for 
each topic.

twtSentimentAnalysis.py
Uses VADER to determine the seniments of each tweet: categorized as neg, neu, or pos.

twtPlotEachTweet.py
Uses folium to plot each tweet as a marker on a map of the US and colored to their
respective sentiment classification: neg = red, neu = gray, pos = green.

twtPlotEachCity.py
Groups all the tweets together by city. Keeps track of how many neg, neu, or pos tweets
there are in any given city. Also, plots three makers (1 neg, 1 neu, 1 pos) for each city.
Folium is used to plot each marker on a map of the US. Size of marker is determined by
how many tweets exist for that city. Also, clickable tool tips for each city exist that
display percentages of tweet classifications.

twtCityStats.py
Groups all the tweets together by city. Keeps track of how many neg, neu, or pos tweets
there are in any given city. Outputs a csv file with all this raw data. 
