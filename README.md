# What the Rise of Tik Tok Could Mean for Spotify & the Future of Music Streaming: An First Look

Watching TikTok become wildly popular these past few year and with Spotify being one of the most popular streaming services, it led me to wonder how exactly Tik Tok has affected music streaming and artist and song popularity. Does this platform really have a noticeable impact on popular music, or are these cases rare? I decided to perform an exploratory data analysis to help visualize and better understand the correlation between what songs are promoted on the Tik Tok algorithm and what is popular on Spotify.

# Project Goals

The main questions I want to answer: 
- Does TikTok have a significant influence on what songs become popular on Spotify?

- If there is a correlation or relationship between “tik tok famous” songs and songs on the top charts, how has it changed as the app continues to grow? 

- And finally, how could this new social media platform change things for Spotify? 

# Data Analysis, Initial Thoughts, and Summary of Process

I used the Spotify API, pandas, matplotlib, and the spotipy libraries to generate my data. A Spotify search led me to playlists of [songs viral on Tik Tok in 2020](https://open.spotify.com/playlist/65LdqYCLcsV0lJoxpeQ6fW?si=iSU447kiTCuQUz-rYz7Dzw), and [songs viral on Tik Tok in 2018](https://open.spotify.com/playlist/73Q2uot60f3KH9N3YolDfV?si=U1Wth-l5QR--fZoyBSteSA). I chose the playlists with the most followers as an indicator of an accurate playlist. I did the same to find the top songs overall for 2020 and 2018. To have data sets of equal sizes, I had to manually merge two “top songs of the year” playlists to get similar sample sizes.

After creating my dataframes, I generated histograms to compare distributions for audio features for Top Tik Tok songs against that of Top Overall songs. The orange histograms are for the Overall Top Songs of the year, and blue for Tik Tok songs. 

My overall observations: 
- For the year 2020, with the exception of song length and tempo, the distributions for each audio feature seems to have very tight overlaps. The types of sounds, features, and thus songs that seem to be popular in one data set correlate well with the other. 
- Tempo having a higher frequency in the Tik Tok data set might be influenced by the larger sample (160 vs 139).
- Song length is interesting: songs popular on Tik Tok seem to be noticeably shorter than the charts. This could be due to the fast-viral-and-short video type content that is the core of Tik Tok. The types of songs that tend to be longer may not have the viral qualities that are often needed to blow up on the app.
- For the year 2018, we see much more variance between distributions, particularly for energy, loudness, valence, and length. Songs on Tik Tok have a greater range in energy, greater range in loudness, slightly higher valence and slightly shorter length. The types of sounds popular on Tik Tok are thus less tightly correlated with the top charts.





