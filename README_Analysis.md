# Spotify Audio Features vs Popularity Analysis and Conclusion

**Contributors:** Richard Bialick, Julio Dela Cruz, Tim Haake, Kylie Li, Nancy Zheng  
**Link to Github Repo:** https://github.com/zhengn95/
[Presentation Link](https://docs.google.com/presentation/d/179E6XyXVGUQcURvWDIAINpz7rKUUxUfqtZ6FTdYGt7I/edit?usp=sharing)
#### Project Description:
In our project, we analyzed different audio features that may contribute to the popularity of the top tracks from [Top 10 Streamed Artists in the United States on Spotify](https://open.spotify.com/section/0JQ5DAnM3wGh0gz1MXnu3C). We made conclusions on current and future trends based on comparing various audio features to music popularity.

#### Research Questions:
How is the popularity of the top tracks of the Top 10 Streamed Artists on Spotify  affected by audio features such as acousticness, tempo, energy, loudness, speechiness, danceability, and valence?  

Using the correlation between popularity and audio features, what can we predict about future music trends?  

#### Datasets Used:
[Spotify Web API](https://developer.spotify.com/documentation/web-api)  
[The Top 10 Artists Globally in 2023](https://newsroom.spotify.com/2023-11-29/top-songs-artists-podcasts-albums-trends-2023/)  

**Top 10 Artists Streamed on Spotify in the United States - Artist ID numbers**

1. Taylor Swift - https://open.spotify.com/artist/06HL4z0CvFAxyc27GXpf02?si=28979011a2f446fb
2. Drake - https://open.spotify.com/artist/3TVXtAsR1Inutravj472S9r4?si=c036ec885a6c4ab7
3. Travis Scott - https://open.spotify.com/artist/0Y5tJX1MQlPlqiwlOH1tJY?si=13b2ea9ddc304c14
4. Zach Bryan - https://open.spotify.com/artist/40ZNYROS4zLfyyBSs2PGe2?si=db0c9492a4a44e5c
5. Kanye West - https://open.spotify.com/artist/5K4W6rqBFWDnAN6FQUkS6x?si=14d9933251a04f4e
6. The Weeknd - https://open.spotify.com/artist/1Xyo4u8uXC1ZmMpatF05PJ?si=7fd262759d3d453f
7. Morgan Wallen - https://open.spotify.com/artist/4oUHIQIBe0LHzYfvXNW4QM?si=7c693b6829d04717
8. 21 Savage - https://open.spotify.com/artist/1URnnhqYAYcrqrcwql10ft?si=f620ac02e71c485e
9. Bad Bunny - https://open.spotify.com/artist/4q3ewBCX7sLwd24euuV69X?si=aad3dd7099f742bf
10. Future - https://open.spotify.com/artist/1RyvyyTE3xzB2ZywiAwp0i?si=876369688ab64a7d**Track ID 

**API Endpoint to Extract Audio Features**  
track_href': https://api.spotify.com/v1/tracks/{Track ID}  
analysis_url': 'https://api.spotify.com/v1/audio-analysis/{Audio Analysis ID}  

*Note: Please see the Python notebook for the Track IDs and Audio Analysis IDs for each top track *

#### Rough Breakdown of Tasks:

**Tasks:**
- Data extraction from Spotify API by requesting data using python 
- Cleaning data and format into data frames 
- Merging data frames
- Statistical analysis using linear regression & correlation with the dependent variable (y) as Popularity
- Statistical analysis using boxplots and summary statistics of each audio feature
- Update the main branch via commit and merge each member's analysis in GitHub
- Write-up & slide Deck of the analysis

**Ricky Bialick:** 
- Data authentication of Spotify API
- Plot correlation & regression line between Loudness vs Popularity with the conclusion of the analysis 
- Statistical analysis using boxplots and summary statistics for loudness

**Julio Dela Cruz:**
- Plot correlation & regression line between Danceability vs Popularity with the conclusion of the analysis
- Statistical analysis using boxplots and summary statistics for danceability
- Plot correlation & regression line between Energy vs Popularity with the conclusion of the analysis  
- Statistical analysis using boxplots and summary statistics for energy

**Tim Haake:**
- Data extraction from Spotify API
- Data cleaning & format into data frames
- Plot correlation & regression line between Acousticness vs Popularity with the conclusion of the analysis
- Statistical analysis using boxplots and summary statistics for acoustics

**Kylie Li:**
- Plot correlation & regression line between Valence vs Popularity with the conclusion of the analysis
- Statistical analysis using boxplots and summary statistics for valence
- Plot correlation & regression line between Speechiness vs Popularity with the conclusion of the analysis  
- Statistical analysis using boxplots and summary statistics for speeches
- Merging tables  

**Nancy Zheng:**
- Proposal, write-up, and slide deck draft & edits
- Defined regression plot & boxplot functions 
- Plot correlation & regression line between Tempo vs Popularity with the conclusion of the analysis
- Statistical analysis using boxplots and summary statistics for tempo

#### Summary and Conclusions
The top tracks of the top streaming artists on Spotify on January 17, 2024 do not appear to be  affected by audio features.
The correlation coefficient (r) showed a very weak or no correlation across all audio features when compared with popularity of tracks. We can conclude that the specified audio features are unlikely to affect popular music and future trends in music.

#### Limitations 
- Limited to popular music vs other genres
- Limited specific audio features vs all audio features
- Limited to only Top Tracks in the United States vs Globally
- Limited to top 10 artists and their top tracks vs all music on Spotify
- Performed Linear Regression and Pearson’s Correlation only vs Chi-Square and other tests for significance

