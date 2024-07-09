**Introduction*
-

- Note! This dataset is taken from Kaggle by `NIDULA ELGIRIYEWITHANA`, top 1000 streamed Spotify songs on 2023. 

- This study analyzes the top 1000 streamed songs on Spotify to investigate whether the type of artist—solo, duo, or group—affects streaming performance and whether any variables listed below will contribute to a song's success. Utilizing data from these top tracks, I categorize each song by streaming counts into ranks - top 10, top 100, and top 500 to determine trends across different artist types. I will answer three questions, which are evaluated from the main question.


**Question:**
-
- `Main Question`: Artist impact: Analyze how artist involvement and attributes relate to a song's success.

  1. How does the performance vary among solo artists, duos, and groups within the top 10, top 50, top 100, and top 500 ranked songs on Spotify?

  2. What song characteristics like key and bpm within the top 10, top 50, top 100, or top 500?
  
  3. Does the release date of a song correlate with its streaming success?

**Results**
-
**Question 1**

**Hypothesis**
-
1. Songs with multiple artists perform better on streaming platforms than songs by solo artists.



**Variables**
-
 - **response variable**
      - `streams` - Total number of streams on Spotify
 - **Observer**
      - `artists_name`
      - `in_spotify_playlists` - Number of Spotify playlists the song is included in

      - `in_spotify_charts` - Presence and rank of the song on Spotify charts

      - `bpm` - Beats per minute, a measure of song tempo

      - `key`

      - `mode` - Mode of the song (major or minor)

      - `danceability_%` - Percentage indicating how suitable the song is for dancing

      - `valence_%` - Positivity of the song's musical content

      - `energy_%` - Perceived energy level of the song

      - `acousticness_%` - Amount of acoustic sound in the song

      - `liveness_%` - Presence of live performance elements

      - `speechiness_%` - Amount of spoken words in the song

      - `released_date`
      
      - `artists_type` - Solo (artists_count = 1), Duo (artists_count = 2), Group (artists_count > 3)

**Methodology**
 - Collect data 
    - From "top-spotify-songs-2023" (Kaggle)
 - Wrangle data 
    - Cleaning
         - Remove variables that are not related to our topic(Spotify).
         - Remove any rows with empty data
 - Explore 
    - data using available techniques
 - Visualization
    - data to uncover insightful discoveries
