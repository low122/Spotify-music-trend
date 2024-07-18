**Introduction*
-

- Note! This dataset is taken from Kaggle by `NIDULA ELGIRIYEWITHANA`, top 1000 streamed Spotify songs on 2023.

- This study analyzes the top 1000 streamed songs on Spotify to investigate whether the type of artist—solo (1), duo (2), or group—affects (3) streaming performance and whether any variables listed below will contribute to a song's success. Utilizing data from these top tracks, I categorize each song by streaming counts into ranks - top 10, 50, 100, 250, 500, 650, 817 to determine trends across different artist types. I will answer three questions, which are evaluated from the main question.


**Question:**
-
- `Main Question`: Artist impact: Analyze how artist involvement and attributes relate to a song's success.

  1. How does the performance vary among solo artists, duos, and groups within the top 10, 50, 100, 250, 500, 650, 817 ranked songs on Spotify?

  2. What song characteristics like key and bpm within the top 10, 50, 100, 250, 500, 650, 817?

**Results**
-

**Question 1**
- Based on the analysis, despite duos (2 artists_count) having a significant proportion in the Top 10, but solo (1 artists_count) streams surpassing duo streams by 15%. Moreover, solo artists consistently achieve higher total streams within the ranked. This indicates a stronger performance impact from solo artists within the top-ranked songs on Spotify.

**Key Findings**
-
**Question 1**
- Based on the analysis, despite duos (2 artists_count) having a significant proportion in the Top 10, but solo (1 artists_count) streams surpassing duo streams by 15%. Moreover, solo artists consistently achieve higher total streams within the ranked. This indicates a stronger performance impact from solo artists within the top-ranked songs on Spotify.

**Question 2**
 - **BPM**
   - BPM does not change much across the ranks, but some valuable information remains.

   - The overall average BPM in each rank is in the range [117, 125].

   - The best BPM range observed in the Top 10 is in [90, 110] (majority).

      - The standard deviation in the top 10 is the highest (33) among all the ranks

         - Majority (6 songs) average key value in the top 10 is 96.5
         
         - Minority (4 songs) average key value in the top 10 is 149.5

- **Keys**
   - **Overall Distribution (across all ranks):**

      - C# has the largest proportion 14% in total

      - D# has the smallest proportion 3.68%

      - The proportion of A, B, D, F, F#, G, G# are in the between [8.58%,11.15%]

      - A# and E takes 6.74% and 7.23% respectively

   - **Distribution by Ranking:**

      - C# takes majority in Top 10 (30%) and Top 50 (22.50%)

      - F, E, B, D#, F# do not show up in the top 10 songs
      
      - A does not show up in the top 50 songs

- **Mode**
   - **Overall Distribution (across all ranks):**

      - The dataset contains 451 songs in Major mode and 365 in Minor mode. Major mode exceeds Minor by 19.07%.

   - **Distribution by Ranking:**

      - Top 10 to Top 650: 
         - Major mode predominates in all these rankings.

      - Proportional Decline: 
         - The proportion of songs in Major mode gradually decreases from the Top 10 through the Top 650. The highest proportion is 70% in the Top 10, decreasing to a minimum of 54.67% in the Top 650.

      - Shift in Top 817: 
         - In contrast, the Top 817 ranking shows a slight majority for Minor mode, with 51.20% of songs, compared to 48.80% for Major.

- **Danceability**
    - Overall: Generally ranges between 70% to 80%.

    - Top 10: 
       - Maximum is 83%, average is 69.10%, similar to Top 650. Standard deviation is 12.83%, indicating moderate variability.

    - Top 50 to Top 817: 
      - Maximum danceability consistently around 95-96%, suggesting a strong preference for highly danceable tracks.

 - **Valence**
    - Overall: Typically between 45% and 55%, with a consistent standard deviation of ~23.47 across rankings.

    - Top 10: Highest average valence at 59.40%, closely followed by Top 650 at 55.59%.

    - Other Rankings: Averages generally lie between 46.90% and 49.81%.

- **Energy**
    - Overall: Ranges from 60% to 65%.

    - Top 10: Lowest maximum energy at 78%, minimum at 45%, and the lowest average of 59.60% with a standard deviation of 10.97.

    - Other Rankings: Maximum values frequently above 90%, with minimums sometimes dropping below ~30%. Averages fall between 63.62% and 65.68%.
    
- **Acousticness**
    - Overall: Generally around 20% to 28%.

    - Top 10: Maximum at 69%, minimum at 1%.

    - Other Rankings: Maximum values can reach above 90%; minimum consistently at 0%.

- **Instrumentalness**
    - Overall: Ranges broadly from 0% to 2%.

    - Top 10: Both maximum and minimum values are 0%.

    - Top 50 to Top 500: Maximum value rises sharply from 11% to 91%.

    - Top 500 and Top 817: Peaks at 91% and 83%, respectively, indicating significant tracks with high instrumental content.

- **Liveness**
    - Trends: 
      - Maximum liveness increases significantly from Top 10 to Top 817, with a dramatic peak of 97% in Top 250.

    - Consistency: 
      - Minimum liveness remains nearly zero across all ranks, indicating many studio-produced tracks.

    - Average: Stays around 15% to 20%, with moderate variability.

- **Speechiness**
    - Progression: Noticeable increase in maximum speechiness from Top 10 to Top 817.

    - Consistency: Minimum speechiness remains around 2-3% across all ranks.

    - Stability:
       - Mean speechiness ranges from about 7% to 12%, with lower standard deviations except for fluctuations in mid-rankings (Top 100 to Top 650).


**Hypothesis**
-
1. Songs with multiple artists perform better on streaming platforms than songs by solo artists.



**Variables**
-
 - **response variable**
      - `streams` - Total number of streams on Spotify
 - **Observer**
   - **Numeric**
      - `artists_name`

      - `bpm` - Beats per minute, a measure of song tempo

      - `danceability_%` - Percentage indicating how suitable the song is for dancing

      - `valence_%` - Positivity of the song's musical content

      - `energy_%` - Perceived energy level of the song

      - `acousticness_%` - Amount of acoustic sound in the song

      - `liveness_%` - Presence of live performance elements

      - `speechiness_%` - Amount of spoken words in the song

      - `released_date`

   - **Category**
   
      - `key` - Key of the song

      - `mode` - Mode of the song (major or minor)
      
      - `artists_type` - 1 (artists_count = 1), 2 (artists_count = 2), 3 (artists_count > 3)

**Methodology**
-
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


**References**
-
- `FGJSPACEMAN`, title : `♫ Spotify 1 - What Does It Take to Hit the Charts`
