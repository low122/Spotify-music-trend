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
   - BPM does not change much among the ranks, but some valuable information remains.

   - The overall average BPM in each rank is in the range [117, 125].

   - The best BPM range observed in the Top 10 is in [90, 110] (majority).

      - The standard deviation in the top 10 is the highest (33) among all the ranks

         - Majority (6 songs) average key value in the top 10 is 96.5
         
         - Minority (4 songs) average key value in the top 10 is 149.5

   - Consider BPM with a mean of larger than 125:

      - Two outlier songs in top 10 have a mean of 178 BPM, which is a leading component among all the ranks

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
