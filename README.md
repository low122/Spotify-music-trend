**Spotify Music Trend Analysis 2023**
-

**Project Background**

This project focuses on analyzing the top 1000 streamed songs on Spotify in 2023, exploring key features that influence song rankings and performance. The goal is to understand trends in song features, artist types, and their correlation with stream counts, ultimately providing insights into what makes a song "trendy." The analysis leverages data analytics tools and methodologies to categorize and rank songs, uncover feature-based trends, and offer recommendations.

- Insights and recommendations are provided on the following key areas:

1. Song Features (e.g. BPM, Danceability, Valence, Energy)

2. Artist Composition (Solo, Duo, Group)

3. Key and Mode Trends (e.g., D#, Major)

4. Ranking-Based Transformations (Streams to Rank Categories)

- **Data Structure & Initial Checks**

    - The dataset consists of key song features and rankings from Spotify’s top 1000 streamed songs in 2023. Each song was analyzed for streams, features, and ranking, with an emphasis on identifying patterns across ranked categories.

![Uploading Screenshot 2025-01-03 at 21.24.21.png…]()

- **Executive Summary**

    - **Overview of Findings**

        - Streams: Streams were transformed into rank categories (Top 10, Top 50, etc.) to better capture trends, as raw stream counts lacked significant correlations with individual features.

        - Artist Type: Solo artists contributed approximately 60% of the top-ranked songs, significantly outperforming groups (~12%).

        - Key and Mode: While the D# key had the lowest proportion of songs (~3.67%), it significantly boosted performance when combined with Major mode (48% higher streams).

        - Feature Insights: BPM and danceability emerged as key distinguishing features for higher-ranked songs, while valence and energy maintained consistency across ranks.

    - **Insights Deep Dive**

        - Category 1: Song Features (BPM, Danceability, Valence, Energy)

            - **BPM (Beats Per Minute)**

                - Main Insight 1: The range (25th to 75th percentile) of BPM fluctuates across ranks, with higher ranks exhibiting narrower distributions.

                - Top 10: Median BPM ~116.5.

                - Top 100–Top 817: Median BPM rises to ~125.5.

                - Supporting Observation: BPM is highly informative in distinguishing higher-ranked songs (Top 10) from lower ranks.

            - **Danceability**

                - Main Insight 2: Danceability ranges from 60% to 78% across all ranks, with the Top 10 showing slightly higher averages (~69.1%).

                - Maximum values stabilize (~95%) across most rankings, reflecting strong market preference for high danceability.

            - **Valence**

                - Main Insight 3: Valence displays a broad spread (25.5% to 76.25%), with Top 10 songs favoring higher emotional positivity (median ~56.5%).

                - Middle Ranks (Top 50–Top 250): Slightly lower valence (~48%), indicating more neutral tones.

            - **Energy**

                - Main Insight 4: Energy levels remain high across ranks (48.75% to 79.25%), with Top 10 songs showing slightly lower median energy (~57.5%) compared to middle ranks (~68%).

                - Top 50–Top 100: Exhibit the highest variability, reflecting more energetic tracks.

            - **Acousticness, Liveness, and Speechiness**

                - Main Insight 5: After implement the ranking, the transformation of acousticness, liveness, and speechiness from left-skewed to right-skewed distributions underscores the importance of ranking-based analysis.

                - This transformation shifts the focus to higher-end values (e.g., the 75th percentile), enhancing the predictive power of these features for distinguishing Top 10 songs from lower ranks.

                - Their shared characteristics further emphasize their potential in analyzing and predicting song performance across rankings.



    - **Category 2: Artist Composition**

        - Solo vs. Group Artists

        - Main Insight 1: Solo artists contribute ~60% of top-ranked songs, with group artists contributing only ~12%.

        - Supporting Observation: Solo artists dominate the Top 10 and Top 50 rankings, indicating stronger performance across all features.





    - **Category 3: Key and Mode Trends**

        - Key (D#) and Mode (Major)

        - Main Insight 1: D# is the least common key (~3.67%) but significantly improves streams when combined with Major mode.

            - Improvement: 48% higher streams compared to D# alone; 27.5% compared to Major mode alone.

        - Main Insight 2: Major mode dominates (~55%) across all rankings, consistently outperforming Minor mode.





    - **Category 4: Ranking-Based Transformations**

        - Streams to Rank Categories

        - Main Insight 1: Transforming streams into rank categories (Top 10, Top 50, etc.) revealed clearer trends compared to raw streams.

        - Main Insight 2: Features like BPM and danceability are more effective in predicting rank categories compared to raw stream counts.





- **Recommendations**

    - Based on the insights and findings above, we recommend the following:

    1. Prioritize High Danceability: Ensure songs target danceability values between 60% and 78%, with a preference for ~95% in higher ranks.

    2. Focus on Emotional Positivity: Favor songs with higher valence (~56%) for the Top 10, appealing to broader audiences.
    
    3. Leverage D# Key with Major Mode: Despite its rarity, combining D# with Major mode significantly boosts performance.

    4. Target Solo Artists: Promote solo artists, as they dominate higher-ranked songs.
