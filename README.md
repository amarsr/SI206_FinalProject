# Music Trends Over Time

Requires python package [spotipy], [sqlite3], [Billboard], [googleapiclient.discovery], [beautifulsoup], [paralleldots]

Run `pip3 install spotipy` to install [spotipy]
Run 'pip install billboard' to install [billboard]
Run 'pip install --upgrade google-api-python-client' to install [googleapiclient.discovery]
Run 'pip install paralleldots' to install [paralleldots]
Run 'pip apt-get install python3-bs4' to install [beautifulsoup]

# Database

The database is titled SIfinal.sqlite and contains data on the following attributes for the top 110 songs from the past 29 years:
    - BPM
    - Danceability
    - Song Name
    - Artist
    - YouTube Views
    - Lyrics
    - Probability of Intended Sentiment

# Spotify_Data_Collect

This file will require you to have a clientid and a clientsecret code that you will have to obtain from Spotify.com/developer

Input these codes into a seperate file and import that file to spotify_data_collect.py

If spotipy is downloaded, this should output key measures


# Billboard

This file will required you to have the billboard package installed 

Input put a YYYY/MM/DD combination to receive the top 10 songs from that week and write them to a database

Everytime the file is run, the user should add 10 to the ID variable to maintain unique identifers in the database

# Youtube 

This file will require you to have the googleapiclient.discovery package to be installed 

Input is a song and artists pair that is drawn from a database

# GetLyriccs

This file also requires the googleapiclient.discovery package and the paralleldots package to be installed

The genius API requires a artist and song as inputs a returns a string of lyrics. These lyrics are then passed into the paralleldots sentiment analyzer and a sentiemnt score is reutrned

# Visualizations

Run this file to output 5 visuals depicting trends for views, danceability, views over time, etc...

