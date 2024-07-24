**Introduction*
-

- Note! This dataset is taken from Kaggle by `NIDULA ELGIRIYEWITHANA`, top 1000 streamed Spotify songs on 2023.

- This study analyzes the top 1000 streamed songs on Spotify to investigate whether the type of artist—solo (1), duo (2), or group—affects (3) streaming performance and whether any variables listed below will contribute to a song's success. Utilizing data from these top tracks, I categorize each song by streaming counts into ranks - top 10, 50, 100, 250, 500, 650, 817 to determine trends.


**Question:**
-
- `Main Question`: Artist impact: Analyze how artist involvement and attributes relate to a song's success.

  1. How does the performance vary among solo artists, duos, and groups within the top 10, 50, 100, 250, 500, 650, 817 ranked songs on Spotify?

  2. How is it different between the songs in the top 10 and the top 50, according to this dataset?

**Results**
-

**Question 1**
- Based on the analysis, despite duos (2 artists_count) having a significant proportion in the Top 10, but solo (1 artists_count) streams surpassing duo streams by 15%. Moreover, solo artists consistently achieve higher total streams within the ranked. This indicates a stronger performance impact from solo artists within the top-ranked songs on Spotify.

**Question 2**
 - Top 10 Characteristics:
     - BPM: Averages 117-125, with a focus around 90-110.

     - Mode: Major mode dominates (70%).

     - Danceability: High, averaging 69.10%, peaking at 83%.

     - Key: C# is the most frequent.

     - Energy: Lower average at 59.60%, ranges 45-78%.

     - Acousticness: Ranges from 1% to 69%.

     - Speechiness: Low, with a maximum of 28%.

 - Top 50 Characteristics:
    - BPM: Consistently averages 117-125.

    - Mode: Major mode prevalent (66.5%).

    - Danceability: Very high, peaks near 95-96%.

    - Key: Good variety, with C# still common.

    - Energy: Generally higher, more dynamic.

    - Acousticness: Less acoustic than Top 10.
    
    - Speechiness: Slightly higher, up to 37%.


**Findings**
-

- Based on the analysis, despite duos (2 artists_count) having a significant proportion in the Top 10, but solo (1 artists_count) streams surpassing duo streams by 15%. Moreover, solo artists consistently achieve higher total streams within the ranked. This indicates a stronger performance impact from solo artists within the top-ranked songs on Spotify.

 - **BPM:**

    - **Overall Range:** 117 to 125 BPM across all ranks.

    - **Top 10:** Majority of songs have BPM between 90 and 110, indicating a preference for moderately paced tracks.

    - **Variability:** Highest standard deviation in Top 10 (33), indicating more variability in song tempo within top-ranked songs.

- **Key:**

    - **Predominant Keys:** C# is prevalent in the Top 10 (30%) and Top 50 (22.50%).

    - **Notable Absences:** Keys such as F, E, B, D#, and F# are missing in the Top 10; A is missing in the Top 50.

- **Mode:**

    - **Majority Mode:** Major mode dominates from Top 10 to Top 650.

    - **Proportional Shift:** Major mode decreases from 70% in Top 10 to 54.67% in Top 650, with Minor mode overtaking in Top 817 (51.20%).

- **Danceability:**

    - **General Trend:** Ranges from 70% to 80%. Top 10 features high consistency with a mean of 69.10%, and peaks in danceability appear consistently high (95-96%) from Top 50 to Top 817.

- **Energy:**

    - **Variation:** Energy levels show less variation in Top 10 with a low of 45% and high of 78%, compared to higher peaks (above 90%) and lower troughs (below 30%) in other rankings.

- **Acousticness:**

    - **Top 10:** Shows higher acousticness with a max of 69%.

    - **Other Rankings:** Maximum values frequently exceed 90%, with consistent minima at 0%.

- **Instrumentalness:**

    - **General Trend:** Remains low across most rankings but spikes in Top 500 and Top 817, suggesting an increase in instrumental tracks.

- **Liveness:**

    - **Dramatic Peak:** Peaks at 97% in Top 250, indicating some highly live-recorded tracks in mid-to-lower rankings.

- **Speechiness:**

    - **Increasing Trend:** Rises significantly from Top 10 (max 28%) to Top 817 (max 64%), reflecting more vocal content in lower rankings


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
 - Data Wrangling

   - Cleaning:
      - Removed irrelevant variables not directly associated with our analysis of Spotify's data.
      
      - Eliminated any rows containing missing or incomplete data to ensure consistency.

   - Data Exploration

      - Use built-in functions in pandas to determine data type and use plot and seaborn to show statistical data of each variable.

   - Ranking Methodology

      - Categorized songs based on their streaming numbers, allowing for a structured analysis of song popularity across different tiers of streaming success.

 - Data Visualization

    - Implemented visual tools (matplotlib, seaborn) to illustrate the data, aiming to effectively highlight key insights and trends.

**References**
-
- `FGJSPACEMAN`, title : `♫ Spotify 1 - What Does It Take to Hit the Charts`
