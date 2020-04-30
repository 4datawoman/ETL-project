# etl-project

ETL Project

Objective: 
To gather datasets from major media platforms such as Youtube, Spotify, MusicBrainz, Last.fm, and Billboard top charts in order to extract different popularity measures throughout the years. We want to gather data regarding top trending songs, artists, and genres.

“Scrobble” is the idea of sending information regarding the music you are listening to to suggest similar music through your service provider. This data  may have an effect on music trends.

Extraction
We gathered various datasets from Kaggle and other sources. Our datasets ranged from 360MB to 5MB. 
Media Platform
Data Extract
Billboard
Artist
Song

MusicBrainz and Last.fm
Artist
Genre

Spotify
Top 200
Artist
Song
Stream

Youtube
Music videos
Views
Artists
Songs

Data Sources:
https://www.kaggle.com/datasnaek/youtube (NN)
https://www.kaggle.com/edumucelli/spotifys-worldwide-daily-song-ranking (NN)
https://www.kaggle.com/pieca111/music-artists-popularity (TC)
https://www.kaggle.com/miteshsingh/hollywood-music-dataset (TC)









Transformation
Our initial steps were to read our data frames and remove columns that were irrelevant to our overall goal.


We only wanted data from the US region for measures of popularity


We extracted the various genre type attributed to different artists


After cleaning the datasets, we merged the csv files to create dataframes based on:
Measures of popularity
Artists and songs
Artists and genre tags

Figure 1. Measures of Popularity






Load
We chose to use NoSQL utilizing MongoDB to load our tables into a database. We create 3 tables as listed above.

Different table view samples:
. 






